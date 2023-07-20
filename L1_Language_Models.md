# L1 Language Models, the Chat Format and Tokens

## Setup

```py
import os
import openai
import tiktoken
from dotenv import load_dotenv, find_dotenv
_ = load_dotenv(find_dotenv()) # read local .env file

openai.api_key  = os.environ['OPENAI_API_KEY']
```

### helper function

```py
def get_completion(prompt, model="gpt-3.5-turbo"):
    messages = [{"role": "user", "content": prompt}]
    response = openai.ChatCompletion.create(
        model=model,
        messages=messages,
        temperature=0,
    )
    return response.choices[0].message["content"]
```

## Prompt the model and get a completion

```py
response = get_completion("What is the capital of France?")
print(response)
```

## Tokens

```py
response = get_completion("Take the letters in lollipop \
and reverse them")
print(response)
```

#### "lollipop" in reverse should be "popillol"

```py
response = get_completion("""Take the letters in \
l-o-l-l-i-p-o-p and reverse them""")
print(response)
```

## Helper function (chat format)

### Helper function

```py
def get_completion_from_messages(messages, 
                                 model="gpt-3.5-turbo", 
                                 temperature=0, 
                                 max_tokens=500):
    response = openai.ChatCompletion.create(
        model=model,
        messages=messages,
        temperature=temperature, # this is the degree of randomness of the model's output
        max_tokens=max_tokens, # the maximum number of tokens the model can ouptut 
    )
    return response.choices[0].message["content"]
```

```py
messages =  [  
{'role':'system', 
 'content':"""You are an assistant who\
 responds in the style of Dr Seuss."""},    
{'role':'user', 
 'content':"""write me a very short poem\
 about a happy carrot"""},  
] 
response = get_completion_from_messages(messages, temperature=1)
print(response)
```


