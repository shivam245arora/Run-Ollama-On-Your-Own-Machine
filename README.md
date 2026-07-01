<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Run Ollama On Your Own Machine

**Project Link:** [View Project](http://nextwork.ai/projects/ai-ollama-setup)

**Author:** Shivam Arora  
**Email:** arorashivam419@gmail.com

---

![Image](http://nextwork.ai/positive_blue_glamorous_sloth/uploads/ai-ollama-setup_n1p5r9t3)

---

## Introducing Today's Project!

In this project, I'm going to install Ollama in my system and run AI locally. 
This will help me to understand how AI works locally and what things it is capable of. 
I'm interested in this because I love everything about the AI and how it is implemented, and I want to learn more and more.

### Key tools and concepts

The key tools are
I used Ollama to manage and run large language models locally; PowerShell/Terminal to interact with the models via CLI commands (ollama pull, ollama run, ollama list); and Notepad to configure a custom Modelfile

Key concepts I learned are how local LLMs differ from cloud APIs in terms of data privacy and offline capability; the parameters size trade-offs (e.g., 0.5b vs 1b); how Retrieval-Augmented Generation (RAG) bridges the gap for custom data access; and how system prompts define custom AI personas without the need for retraining.

### Challenges and wins

This project took me approximately 30-45 minutes.
The most challenging part was understanding the difference between system prompts (which define a model's persona) and RAG (which defines what data the model can access), as well as setting up the Modelfile syntax correctly in Notepad. It was awesome to see the coding-tutor persona come to life right inside my terminal!"

---

## Installing Ollama for Local AI

In this step, I'm going to install Ollama on my system. 
Ollama is an open-source platform that lets you download, run, and manage large language models (LLMs) directly on your own computer. It simplifies the process, providing a command-line interface and a local API to easily use AI models offline, ensuring privacy and control.

![Image](http://nextwork.ai/positive_blue_glamorous_sloth/uploads/ai-ollama-setup_h4n8k2m6)

### Verifying the installation

I verified Ollama is running by using the curl request to http://localhost:11434
The response I saw was "Ollama is running..."

---

## Pulling My First AI Model

In this step, I'm going to check our current model and then pull the Qwen2.5:0.5b model.
Then we are going to chat with it!

![Image](http://nextwork.ai/positive_blue_glamorous_sloth/uploads/ai-ollama-setup_b5c9d3f7)

### Understanding model sizes

I pulled the model using 'ollama pull qwen2.5:0.5b'

The 0.5b means the model is small and lightweight  and have fewer parameter than 7b and 70b (400 mb).

---

## Chatting with My Local AI

I chatted with my local AI by running the model using `ollama run {model name}. 

I ask, "What is the capital of India?" It responded with New Delhi with a full description about the place 

This is different from cloud AI because data never leaves my computer.

![Image](http://nextwork.ai/positive_blue_glamorous_sloth/uploads/ai-ollama-setup_n1p5r9t3)

---

## Exploring Local AI Limitations

"In this step, I'm going to discover the limitations of local AI models. We see that while local models are great for privacy, they don't know personal information (like my name) or real-time data out of the box."

![Image](http://nextwork.ai/positive_blue_glamorous_sloth/uploads/ai-ollama-setup_d8r4t6w1)

### Understanding RAG

The base model was only trained on general internet knowledge up to its cutoff date. It doesn't have access to my private files, personal context, or real-time updates. 

RAG stands for Retrieval-Augmented Generation. It solves this by letting the AI search an external knowledge base (like my local documents) to find relevant snippets and use them to answer my questions accurately, without retraining the model.

---

## Creating a Custom AI Persona

In this project extension, I created a persona called a coding-tutor.
It behaves differently because it speaks like a coding teacher, answering in a format everyone can easily understand.

![Image](http://nextwork.ai/positive_blue_glamorous_sloth/uploads/ai-ollama-setup_j3k7m2n8)

---

## Wrapping Up

"I did this project today to learn how to deploy and manage large language models locally on my own machine using Ollama. This completely met my goals! I now understand the trade-offs between model sizes, how to customize an AI's behavior using a Modelfile system prompt, and how technologies like RAG can be used to securely ground a local model in private data."

---

---
