# Architecture Overview

## System Design

The AI Customer Support Chatbot follows a **Retrieval-Augmented Generation (RAG)** architecture:

```
User Query → Intent Classification → Knowledge Base Retrieval → Response Generation → User
```

## Core Components

### 1. Chat Interface Layer
- Handles user input/output
- Manages conversation state
- Provides embeddable widget for websites

### 2. NLP Processing Engine
- **Intent Detection**: Classifies user message into categories (menu, booking, hours, delivery, allergy, etc.)
- **Entity Extraction**: Pulls relevant entities (date, time, party size, dietary requirements)
- **Context Management**: Maintains conversation history for follow-up questions

### 3. Knowledge Base
- Structured JSON data store
- Categories: Menu, Hours, Location, Delivery, Reservations, Dietary Info, Specials
- Business owner can update data without technical knowledge
- Version controlled for audit trail

### 4. Response Generation
- Template-based responses for common queries (fast, consistent)
- LLM-generated responses for complex queries (flexible, natural)
- Fallback to human handoff for unresolvable queries

## Data Flow

1. Customer sends message via chat widget
2. Message is processed by NLP engine
3. Intent and entities are extracted
4. Relevant knowledge base sections are retrieved
5. Response is generated using retrieved context
6. Response is delivered to customer (< 5 seconds end-to-end)

## Deployment Options

| Option | Best For | Setup Time |
|--------|----------|------------|
| Website Widget | Restaurants, Hotels | 30 minutes |
| WhatsApp Integration | Delivery Services | 1 hour |
| Facebook Messenger | Social-first Businesses | 1 hour |
| Custom API | Enterprise Clients | 2-4 hours |
