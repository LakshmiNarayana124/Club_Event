# 🤖 Techeon Club – AI Campus Event Guide

An AI-powered campus event assistant built using **Dify** to help workshop participants access event information through a simple conversational interface.

## 📌 Project Overview

The Techeon Club AI Campus Event Guide is designed to assist students and workshop participants by answering event-related questions.

The chatbot uses Dify's Chatflow and Knowledge Base capabilities to provide structured responses based on the supplied event information.

## 🎯 Objectives

- Provide event schedules and timings.
- Help participants identify event venues.
- Answer questions about workshop topics.
- Share registration and event-related information.
- Reduce repetitive queries handled by event organizers.
- Direct participants to the registration desk when information is unavailable.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Dify | AI chatbot development platform |
| Dify Chatflow | Conversational workflow |
| Knowledge Base | Event information storage |
| LLM | Natural-language question answering |
| Prompt Engineering | Chatbot behaviour and response control |

## 🧠 Chatbot Identity

**Role:** Official Campus Event Guide AI for the Techeon Club workshop.

**Personality:**
- Welcoming
- Conversational
- Well-organized
- Student-friendly

**Primary instruction:** Answer participant questions using only the available event context. Never invent missing information.

## 📚 Knowledge Base

The chatbot uses a desktop text file named `event details.txt` as its knowledge source.

### Knowledge File Content

The file contains:

- Event Name: Smart Campus Hackathon 2026
- Venue: Main Seminar Hall, Block C
- Timings: 09:00 AM – 05:00 PM IST
- Registration: https://bit.ly
- Food Policy: Free lunch tokens distributed at the registration counter at 01:00 PM.

### Knowledge Integration

1. Create a Knowledge Base in Dify.
2. Upload `event details.txt`.
3. Allow Dify to process and index the document.
4. Connect the Knowledge Retrieval node to the Chatflow.
5. Pass the retrieved context to the LLM.
6. Generate answers based on the retrieved information.

## 🔄 Chatflow Workflow

The chatbot follows this basic process:

**User Question → Knowledge Retrieval → LLM Processing → Context-Based Answer → User**

### Workflow Components

| Component | Function |
|---|---|
| User Input | Receives participant questions |
| Knowledge Retrieval | Searches the uploaded event document |
| LLM | Understands the question and prepares an answer |
| Answer Node | Displays the final response |

## 📅 Workshop Information

The Chatflow instructions also define the following workshop details:

- **Event Topic:** Dify Concepts, Chatbots, and Workflows
- **Date:** Wednesday, 11 November 2026
- **Time:** 01:30 PM – 04:30 PM IST

The chatbot is instructed to use these details as fixed event information.

**Important:** The Chatflow instructions and the uploaded knowledge file currently contain different event names and schedules. Verify the intended event details and synchronize both sources before the live workshop.

## ⚙️ Chatbot Behaviour Rules

1. Greet participants enthusiastically.
2. Maintain a friendly and professional tone.
3. Use Markdown formatting, emojis, and bullet points.
4. Answer questions using the supplied context.
5. Never fabricate room numbers, registration information, or other missing details.
6. For unknown information, direct participants to the registration desk organizers.

## 💬 Example Questions

Participants can ask:

- What is the workshop topic?
- When does the workshop start?
- Where is the event taking place?
- What is the event schedule?
- How can I register?
- Are lunch tokens available?
- What will we learn about Dify?

## 🚀 Expected Outcome

The project demonstrates how a no-code AI platform can be used to develop a context-aware campus assistant.

It provides students with an accessible way to retrieve event information while demonstrating practical applications of:

- Generative AI
- Prompt Engineering
- Retrieval-Augmented Generation (RAG)
- Conversational AI
- Workflow Automation

## 👥 Developed For

**Techeon Club – Gopalan College of Engineering and Management**

*Building practical AI solutions through hands-on learning.*

---

⭐ **Let's build on Dify!**
