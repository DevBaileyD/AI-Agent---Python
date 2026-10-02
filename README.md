AI Agent – Python Research Assistant

A Python-based AI research agent built as a learning project following the Tech With Tim – Build an AI Agent From Scratch in Python tutorial.

The project uses an LLM with LangChain and a collection of tools to research user queries, retrieve information from online sources, structure the response, and optionally save the research output to a text file.

Features
Accepts a research query from the user
Uses an LLM to determine how to approach the query
Searches the web using DuckDuckGo
Searches Wikipedia for additional information
Uses custom Python tools
Structures the final response into:
Topic
Summary
Sources
Tools Used
Saves research results to research_output.txt using a custom save_to_text tool
Uses environment variables to securely store API credentials
Uses a Python virtual environment for project dependencies
