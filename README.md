# Conversational AI Chatbot with LangGraph & Gemini
A stateful conversational AI chatbot built using LangGraph's graph-based architecture and powered by Google's Gemini 2.0 Flash model.

## Overview
This project demonstrates a modern approach to building conversational AI agents using LangGraph for orchestration and Google's Gemini 2.0 Flash for natural language understanding and generation. The chatbot maintains conversation history and provides intelligent responses through a clean, graph-based workflow.

## Features
- **Stateful Conversations**: Maintains complete conversation history across multiple turns
- **Graph-Based Architecture**: Uses LangGraph's StateGraph for structured message flow
- **Google Gemini Integration**: Powered by Gemini 2.0 Flash for fast, high-quality responses
- **Automatic Message Management**: Built-in message aggregation and state handling
- **Streaming Responses**: Real-time response generation
- **Type-Safe Implementation**: Uses Python type hints for better code maintainability

## Architecture
- The chatbot follows a simple but effective flow:
            |START → Chatbot Node → END|
- **State Management**: TypedDict stores conversation messages with automatic aggregation
- **Graph Structure**: LangGraph orchestrates the conversation flow
- **LLM Integration**: LangChain connects to Google's Gemini API
- **Message Processing**: Each turn processes the complete conversation history for context-aware responses
