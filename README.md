AI Chatbot with Memory using LangGraph & Groq

 Project Overview
This project is an AI-powered chatbot built using Python, LangGraph, and Groq. It uses the GPT-OSS-20B language model to generate intelligent responses while maintaining conversation history using LangGraph's memory management system.

The chatbot remembers previous messages within the same conversation, allowing users to ask follow-up questions without repeating earlier information.

 Key Features
- AI-Powered Chatbot: Generates responses using GPT-OSS-20B through Groq.
- Conversational Memory: Uses LangGraph's InMemorySaver to maintain chat history.
- State Management: Uses Pydantic BaseModel to define and manage conversation state.
- Message History: Uses Annotated and add_messages to automatically manage conversation messages.
- Graph-Based Workflow: Implements StateGraph with START, chatbot node, and END.
- Multi-Turn Conversations: Supports follow-up questions using a persistent thread ID.
- Command-Line Interface: Allows users to interact with the chatbot directly through the terminal.
- Exit Commands: Users can end the conversation by typing quit, exit, or bye.

 Technologies Used
- Python – Core programming language
- LangGraph – Graph-based AI workflow and state management
- LangChain Groq – Integration with the Groq-hosted language model
- GPT-OSS-20B – Large Language Model
- Pydantic – State validation and data modeling
- InMemorySaver – In-memory conversation checkpointing
- Python-dotenv – Environment variable management

 How It Works
1. The user enters a message through the terminal.
2. LangGraph passes the message into the chatbot state.
3. The chatbot node sends the conversation messages to the Groq LLM.
4. The model generates a response based on the conversation context.
5. LangGraph saves the updated conversation state using InMemorySaver.
6. The chatbot displays the response and waits for the next question.

 What I Learned
Through this project, I gained hands-on experience with LangGraph StateGraph, state management, conversational memory, LLM integration, and building stateful AI applications using Python.

I also learned how checkpointing and thread IDs help maintain conversation history across multiple interactions.

 Future Improvements
- Build an interactive interface using Streamlit.
- Add Google Search integration for real-time information.
- Support multiple conversation threads.
- Integrate persistent memory using SQLite.
- Add document-based question answering using RAG.
