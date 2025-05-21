# AI-Powered-Blog-Generation
In this project, an autonomous AI agent is present which is capable of generating coherent and informative blog content from a given video.Utilizing the principles of Agentic AI—autonomy, tool use, reasoning, and goal-directed behavior, the agent performs a sequence of tasks that include transcribing the video using automatic speech recognition (ASR), extracting key topics, summarizing relevant information, and finally generating a structured blog post. The system is designed to operate independently, requiring minimal human input beyond the initial video link.

Problem Statement:
The rapid proliferation of online video content has created a growing need for converting multimedia into structured textual formats such as blogs, articles, and summaries. However, manual transcription, topic extraction, and blog writing are labor-intensive, error-prone, especially when large volumes of content need to be processed.
Traditional AI models often require significant human supervision and lack the ability to autonomously plan and execute multi-step tasks. This limits their effectiveness in complex scenarios like content creation from unstructured video data.
To address this gap, the problem this project aims to solve is:
"How can we design an autonomous AI agent capable of transforming the content of a video into a well-structured blog post by independently performing transcription, web search, summarization, and generation tasks without continuous human intervention?"

System Architecture:
The architecture of the autonomous blog-generating agent is designed around modular components that collaboratively perform the end-to-end task of transforming a video into a blog post. The agent exhibits agentic behavior by intelligently coordinating multiple tools and processes, including transcription, summarization, and content generation.
Components Description
1. Video Input Module
•	Accepts a video topic and youtube handle.
•	Passes the video to the transcription module.
2. Topic Extraction Module
•	Processes the transcript to identify key topics or questions discussed in the video.
•	Uses NLP techniques such as keyword extraction or summarization.
3. Summarization Module
•	Summarizes the retrieved web content to filter relevant insights.
•	Applies extractive or abstractive summarization (e.g., using LLMs or transformer-based models).
4. Blog Generation Agent
•	Organizes the transcript and summarized search results.
•	Uses an LLM (e.g.gpt-4.1-mini) to generate a structured blog post.

Agent Design:
This project leverages CrewAI, a Python-based multi-agent framework, to build and orchestrate a team of collaborative agents that autonomously generate a blog post from a given video. CrewAI enables the composition of specialized agents, each with defined roles, goals, tools, and responsibilities, working in coordination to achieve the overall objective.
CrewAI Framework Overview
CrewAI allows the definition of:
•	Agents: Independent workers with a specific skill or purpose.
•	Tools: APIs or models used by agents (e.g., transcription, web search).
•	Tasks: Atomic units of work that agents are assigned to perform.
•	Crew: A collection of agents working together in sequence or collaboration.

