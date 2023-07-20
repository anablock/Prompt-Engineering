# Prompt-Engineering
# Awesome Prompts [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/anablock/Prompt-Engineering)

A collection of awesome prompts [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) AI/ML libraries, resources and shiny things.


## Courses
* [Article Summarizer Application using OpenAI's GPT model](https://www.youtube.com/watch?v=vpvtZZi5ZWk&t=423s)
* [Build & Integrate your own custom chatbot to a website (Python & JavaScript)](https://www.youtube.com/watch?v=a37BL0stIuM)
* [ChatGPT Course – Use The OpenAI API to Code 5 Projects](https://www.youtube.com/watch?v=uRQH2CFvedY)
* [Search your data using OpenAI Embeddings](https://www.youtube.com/watch?v=Ef6A1Y4FUbU)

### Pass a JSON string to the OpenAI API
To create a JSON string from a CSV file, you can use the csv module in Python. Here's a step-by-step guide to achieve this:
Install any required packages:
You don't need to install any additional packages, as the csv module is included in the standard library.
Write a Python script to convert the CSV to JSON:

```py
import csv
import json

def csv_to_json(csv_file_path, json_file_path):
    # Create an empty list to store the JSON data
    json_data = []

    # Open the CSV file
    with open(csv_file_path, 'r') as csv_file:
        # Create a CSV reader
        csv_reader = csv.DictReader(csv_file)

        # Iterate through each row in the CSV file and append it to the json_data list
        for row in csv_reader:
            json_data.append(row)

    # Write the JSON data to a file
    with open(json_file_path, 'w') as json_file:
        json.dump(json_data, json_file, indent=4)

# Example usage:
csv_file_path = 'input.csv'
json_file_path = 'output.json'
csv_to_json(csv_file_path, json_file_path)
```

Replace input.csv with the path to your CSV file and output.json with the desired output JSON file path.

Run the Python script:Execute the script using the command python script_name.py in your terminal or command prompt, where script_name.py is the name of the Python file you created in step 2.

This script will read the CSV file, convert its content into a JSON format, and write the resulting JSON data to the specified file.

To pass a JSON string to the OpenAI API, you need to make a request to the API using the requests library in Python. Here's a step-by-step guide on how to do this:

Install the requests library:Run the following command to install the requests library if you don't have it installed already:

```
pip install requests
```

Obtain your OpenAI API key:You'll need your OpenAI API key to authenticate with the API. You can find it in your OpenAI account's API key section. Save it to an environment variable or store it securely in your application.

Write a Python script to make an API request:

```py
import requests
import json

# Set your OpenAI API key
api_key = "your_openai_api_key"

# Define your JSON data
data = {
    "prompt": "Translate the following English text to French: 'Hello, how are you?'",
    "max_tokens": 50
}

# Convert your data to a JSON string
json_data = json.dumps(data)

# Set the API endpoint URL
url = "<https://api.openai.com/v1/engines/davinci-codex/completions">

# Prepare the headers
headers = {
    "Content-Type": "application/json",
    "Authorization": f"Bearer {api_key}"
}

# Make the API request
response = requests.post(url, data=json_data, headers=headers)

# Check if the request was successful
if response.status_code == 200:
    # Parse the response JSON
    response_data = response.json()

    # Extract and print the result
    result = response_data["choices"][0]["text"]
    print("Result:", result.strip())
else:
    print(f"Error: {response.status_code} - {response.text}")
```

Replace your_openai_api_key with your actual OpenAI API key. Modify the data dictionary as needed for your use case.

Run the Python script:Execute the script using the command python script_name.py in your terminal or command prompt, where script_name.py is the name of the Python file you created in step 3.

This script will send the JSON data to the OpenAI API, and the API will return a response containing the generated text. You can parse and use this response as needed. Note that this example uses the davinci-codex engine, but you can replace it with your desired engine (e.g., text-davinci-002, text-curie-002, etc.).

## Storing Embeddings in Postgres

`pgvector` is a Postgres extension that provides support for vector operations, including similarity search and nearest neighbor search. It allows you to store vectors as columns in a database table and perform vector operations on them using SQL queries.

One interesting use case of `pgvector` is to use it in conjunction with OpenAI embeddings. Since `OpenAI embeddings represent words and phrases as high-dimensional vectors`, you can store these vectors in a `pgvector column` and use the extension's similarity search capabilities to find similar words or phrases in a large dataset.

For example, let's say you have a database of customer reviews and you want to find all the reviews that mention a particular product. You could use OpenAI embeddings to represent each review as a vector and store these vectors in a pgvector column. Then, you could perform a similarity search to find all the reviews that are similar to the vector representing the product name.

This approach can be very powerful for applications that involve large amounts of text data, as it allows you to perform complex queries on the data using vector operations. However, it does require some additional setup and configuration compared to traditional SQL queries, so it may not be suitable for all use cases.