# LangChain

User input + base prompt = Prompt Template

## Chain 
Achieve a specific task by linking multiple components together.

Chains allow us to combine multiple components together to create a single, coherent application. For example, we can create a chain that takes user input, formats it with a PromptTemplate, and then passes the formatted response to an LLM. We can build more complex chains by combining multiple chains together, or by combining chains with other components.

## Embedding Path (or Indexing)

1. Document loaders
* Document loaders - extract text from the source documents

2. Text splitters
* Text splitters - split long pieces of text into chunks

3. Embedding models
* Embedding models - convert text to numbers, such that similar meaning texts are closer in numbers to each other

4. Vector stores
* Vector stores - numbers are stored in a database called Vector Database

## Retrieval Process


* https://python.langchain.com/en/latest/modules/chains.html
* [Intro to Chains](https://www.youtube.com/watch?v=Y_O-x-itHaU)



