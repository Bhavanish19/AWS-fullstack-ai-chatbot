
Full-Stack AI Chatbot with Redis, GPT, Python, and FastAPI
Overview
This project is an intermediate full-stack application that demonstrates the development of an AI chatbot capable of real-time Q&A functionality. The chatbot leverages Redis for data storage and real-time communication, GPT-J-6B for natural language processing, FastAPI for building the server, and React for the user interface. This project is designed to help developers understand the complete lifecycle of building and deploying a full-stack application.

Table of Contents

Project Architecture
Features
Technologies Used
Setup and Installation
Usage
Contributing
License
Project Architecture
The application architecture is designed to ensure efficient communication between the client and server, as well as seamless integration with the AI model. Below is an overview of the architecture:

![image](https://github.com/user-attachments/assets/c3ba23c5-7280-44a5-8e49-460db1e3b0fb)


Components
Client/User Interface: Built with React 18, the Chat UI communicates with the backend via WebSockets for real-time interaction.
GPT-J-6B and Huggingface Inference API: Utilizes GPT-J-6B, a generative language model with 6 billion parameters, accessible through the Hugging Face Inference API.
Redis: Redis JSON stores chat data, and Redis Streams handles real-time communication with the Hugging Face API.
WebSockets and Chat API: FastAPI manages the chat server, enabling real-time bi-directional communication.

Features
Real-time Chat: Supports real-time Q&A interaction between users and the AI model.
Scalable Backend: Utilizes Redis for fast and efficient data storage and retrieval.
Open-Source AI: Leverages GPT-J-6B, an open-source language model, for natural language understanding and generation.
Modular Design: The project is divided into distinct modules for easy customization and extension.

Technologies Used
Backend: Python, FastAPI, Redis
Frontend: React 18
AI/ML: GPT-J-6B, Hugging Face Inference API
Communication: WebSockets

Setup and Installation
Prerequisites
Python 3.8+
Node.js 14+
Redis (local or managed instance)
Steps

Clone the Repository:

bash
Copy code
git clone https://github.com/Bhavanish19/fullstack-ai-chatbot.git
cd fullstack-ai-chatbot

Set Up Backend:

bash
Copy code
cd server
python -m venv venv
source venv/bin/activate # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt

Set Up Frontend:

bash
Copy code
cd ../client
npm install

Run the Application:

Backend:
bash
Copy code
cd ../server
uvicorn main:app --reload

Frontend:
bash
Copy code
cd ../client
npm start
