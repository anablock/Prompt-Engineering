# Inferring
Infer sentiment and topics from product reviews and news articles.

To infer means to draw a conclusion based on evidence or reasoning. It involves making an educated guess or interpretation about something that is not explicitly stated or detailed. In this section, we will use GPT-3 to infer sentiment and topics from product reviews and news articles.

```py
import openai
import os

from dotenv import load_dotenv, find_dotenv
_ = load_dotenv(find_dotenv()) # read local .env file

openai.api_key  = os.getenv('OPENAI_API_KEY')

def get_completion(prompt, model="gpt-3.5-turbo"):
    messages = [{"role": "user", "content": prompt}]
    response = openai.ChatCompletion.create(
        model=model,
        messages=messages,
        temperature=0, # this is the degree of randomness of the model's output
    )
    return response.choices[0].message["content"]
```

