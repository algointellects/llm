Prompt Engineering: Creating templates to give more desirable or useful results in accordance from an AI chatbot.
eg- using chatgpt for a complicated task.
Simply a prompt is the text we input to AI models when interfacing with them.

5 principles of Prompt engineering

0. Naive Prompt - Start with a simple prompt that describes the task you want done.
1. Give Direction - Describe tge desired style in detail or reference a relavent persona.
2. Specify Format - Define what rules to follow and the required structure of the response.
3. Provide Examples - Insert a diverse set of test cases where the task was done correctly.
4. Evaluate Quality - Identify errors and rate responses, testing what drives responses.
5. Divide Labor - Split tasks into multiple steps, chained together for complex goals.

# Hallucinations: When an AI chatbot makes up information which might not be factually accurate.

To reduce hallucinations: Write "If you don't have a factual answer, just reply with 'Unable to reply', avoid making up a story and make sure that the output is reliable.

Langchain: A python package to access llms (large language models)

Tokens - a token refers to a unit of text that has been extracted or segmented from a larger body of text. Tokens can be individual words, subwords, or characters, depending on the level of granularity in tokenization.
Tokenization - Sentences are transformed into lots of individual tokens.
Token limit depends on the model we are using to yield results, every model has different token limits and larger token limit models are porgressively more expensive.

Approaches to avoid hitting token limits
* Shortening the prompt.
* Chunking
* Windowed chunks
* Summarization

Standard Text model practices -
  Explain it like I'm five
  Writing clear instructions - 
  	Detailed Instructions
  	Specifying the steps
  	Delimiters
  	Specifying length
  Role prompting
  Ask for context
  question rewriting
  progressive summarization

Pydantic: Library for defining interfaces and types inside of python code

JSON(Java Script Object Notation) - A text format that is language - independant can be used with any programming language.

Ways of summerizing large amount of texts 
->Chains can be used to break and interconnect large texts, eg: chain = load_summerize_chain(llm, chain_type = "stuff")
-> Another method to summerize is by using map reducing technique, eg: chains.mapreduce import MapReduceChain

LLMs can understand and can be enhanced by emotional stimuli.
eg: Do some task like this or i'll lose my job

Meta Prompting: Asking the AI model to generate a prompt for a desired output and then using the generated prompt for better results.
Also can be used to generate code and recycling.

Chain of Thought: Is a way of breaking a problem down into a series if interconnected problems.
Reasoning gets involved, for example instead of giving the answer 5+6 equals 11, it will integrate the problem in a real life scenario like Sam has 5 apples and so on.
