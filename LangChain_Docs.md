# LangChain

User input + base prompt = Prompt Template

## Chain 
Achieve a specific task by linking multiple components together.

Chains allow us to combine multiple components together to create a single, coherent application. For example, we can create a chain that takes user input, formats it with a PromptTemplate, and then passes the formatted response to an LLM. We can build more complex chains by combining multiple chains together, or by combining chains with other components.

## Embedding Path (or Indexing)

1. Document loaders - extract text from the source documents
2. Text splitters - split long pieces of text into chunks
3. Embedding models - convert text to numbers, such that similar meaning texts are closer in numbers to each other
4. Vector stores - numbers are stored in a database called Vector Database

## Retrieval Process
![Prompt Retrieval Process](https://images.ctfassets.net/4x83attbnrpr/6VN3Lg1G5OG8PsuizjuVC/55860ef77de4b78da208fdbde7ff31e7/Screenshot_2023-06-14_at_7.14.35_PM.png)

* https://python.langchain.com/en/latest/modules/chains.html
* [Intro to Chains](https://www.youtube.com/watch?v=Y_O-x-itHaU)



