# AI Agent – Python Research Assistant

A Python-based AI research agent built as a learning project following [Tech With Tim's AI agent tutorial](https://www.youtube.com/watch?v=bTMPwUgLZf0) and [original repository](https://github.com/techwithtim/PythonAIAgentFromScratch).

The project uses an LLM with LangChain and a collection of tools to research user queries, retrieve information from online sources, structure the response, and optionally save the research output to a text file.

## How it works

1. The user enters a research question in the terminal.
2. LangChain sends the question, instructions and available tool definitions to the chosen model.
3. The model can request a tool. Python runs it and returns its result to the model.
4. The agent continues until it produces a final response.
5. A Pydantic parser validates the response's structure.
   
The response contains topic, summary, sources and tools_used. Validating these fields does not verify that the research is accurate.

The tutorial includes web search, Wikipedia lookup and a custom text-file save tool. Only tools included in the agent's tool list are available. Registering a save tool does not automatically save every answer: the model must request it. The tutorial's save function appends timestamped text to research_output.txt.
