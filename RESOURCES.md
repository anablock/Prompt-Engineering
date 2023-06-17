# Resources

## Apps

### AI Web Crawler
* [Github](https://platform.openai.com/docs/tutorials/web-qa-embeddings)

### chatgpt-linux-assistant
* [Github](https://github.com/manno/chatgpt-linux-assistant/tree/main)

### chatgpt-retrieval-plugin
The retrieval plugin includes:
* Support for multiple vector databases providers
* All 4 different authentication methods
* Multiple different API features
* [Docs](https://platform.openai.com/docs/plugins/examples)
* [Github](https://github.com/openai/chatgpt-retrieval-plugin)

The code is a backend API built using FastAPI and Python. It defines endpoints for inserting and querying documents, as well as deleting them. The API uses a datastore that is defined in datastore.factory, and gets instantiated in the startup function.  There is also an authentication middleware in place that checks for a bearer token passed in the header of each request. The token can be set as an environment variable, and is checked against the token in the validate_token function. If the token is missing or invalid, a 401 HTTP error is returned.

### gpt-discord-bot
* [Github](https://github.com/openai/gpt-discord-bot/blob/main/src/base.py)

### pinecone-next-semantic-search
* [Github](https://github.com/anablock/pinecone-next-semantic-search)
* Tech stack: node/js/ts/next.js

### Next.js Boilerplate for a simple ChatGPT Plugin
* [Github](https://github.com/dabit3/nextjs-chatgpt-plugin-starter)
* [Youtube](https://www.youtube.com/watch?v=oedDOaqjPgo&list=TLPQMDkwNjIwMjP87-M429KxWA&index=2)

### Salesforce ai-gateway
* [Github](https://github.com/vkeenan/ai-gateway/tree/v1.5)

### TODO Plugin
* [Github](https://github.com/dabit3/nextjs-chatgpt-plugin-starter)
* [OpenAI Docs](https://platform.openai.com/docs/plugins/introduction)
* [Youtube](https://www.youtube.com/watch?v=oedDOaqjPgo&list=TLPQMDkwNjIwMjP87-M429KxWA&index=2)

* [Brex's Prompt Engineering Guide](https://github.com/brexhq/prompt-engineering)
* [ChatGPT Release Notes](https://help.openai.com/en/articles/6825453-chatgpt-release-notes)
* [GPT best practices](https://platform.openai.com/docs/guides/gpt-best-practices)
* [GPT-4 Technical Report](https://arxiv.org/abs/2303.08774)
* [How to stream completions](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_stream_completions.ipynb)
* [LangChain Hub](https://github.com/hwchase17/langchain-hub/tree/master)
* [OpenAI Cookbook](https://github.com/openai/openai-cookbook/blob/main/apps/chatbot-kickstarter/chatbot.py)
* [Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT](https://arxiv.org/abs/2302.11382)