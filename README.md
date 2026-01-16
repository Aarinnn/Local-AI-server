[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTIgMkM2LjQ4IDIgMiA2LjQ4IDIgMTJzNC40OCAxMCAxMCAxMCAxMC00LjQ4IDEwLTEwUzE3LjUyIDIgMTIgMnoiIGZpbGw9IiNmZmYiLz48L3N2Zz4=&logoColor=white)](https://ollama.ai/)
[![Open WebUI](https://img.shields.io/badge/Open_WebUI-4A90E2?style=for-the-badge&logo=web&logoColor=white)](https://github.com/open-webui/open-webui)
[![WSL](https://img.shields.io/badge/WSL-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://docs.microsoft.com/en-us/windows/wsl/)
[![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://www.linux.org/)
[![Self Hosted](https://img.shields.io/badge/Self_Hosted-00A86B?style=for-the-badge&logo=homeassistant&logoColor=white)](https://github.com/awesome-selfhosted/awesome-selfhosted)


![Local AI Document Summarization](local-ai-server/screenshots/hero-document-summarization.png)

# Local AI Server (Ollama + Open WebUI)


A fully local AI setup running a large language model on personal hardware using Ollama and Open WebUI, without relying on cloud-based AI services.


## Project Overview

This project documents the setup of a self-hosted AI system that runs entirely on a local machine.
The goal was to run and interact with a large language model locally using a browser-based interface, while keeping all inference private and offline.

The system uses a local model server combined with a containerized web interface, allowing users to interact with the AI through a browser without relying on any external AI providers.

The goal of this project was to build a self-hosted AI system that:
- Runs entirely on a local machine
- Uses GPU acceleration when available
- Provides a modern web-based chat interface
- Supports document and PDF summarization
- Keeps inference private (no external APIs)

The system combines:
- **Ollama** as the local model server
- **Docker** to containerize the web interface
- **Open WebUI** for browser-based interaction with the model

---

## Tech Stack

- **Ollama** – Local large language model server  
- **Open WebUI** – Browser-based interface for interacting with the model  
- **Docker** – Containerized deployment of the web interface  
- **WSL2 (Ubuntu)** – Linux environment running on Windows  
- **LLaMA 3** – Local large language model
  
---

## Key Features

- Local LLM execution (no cloud dependency)
- Web-based chat interface
- PDF and document summarization
- GPU-accelerated inference
- Dockerized deployment
- Fully offline and privacy-focused

---
  
## How to Run the Project

### 1. Start the Ollama server
In a WSL terminal:
```bash
ollama serve
```

## To check if Ollama is running:

http://localhost:11434

## In a separate terminal
```bash

docker start open-webui
``` 

## In the browser

http://localhost:8080

## How to stop it 
```bash

docker stop open-webui
``` 

Stop the Ollama server by pressing **Ctrl + C** in the terminal where it is running.


## Screenshot / Guide 

The screenshots below show the full setup process and system in action, including local model execution with Ollama, Dockerized Open WebUI, GPU utilization during inference, and document summarization workflows.


WSL + ollama 

![WSL + Ollama Install](local-ai-server/screenshots/01-wsl-ollama-install.png)

Confirms that ollama is running

![Ollama Running](local-ai-server/screenshots/02-ollama-running.png)

AI running in Terminal + GPU usage ( Side by Side )

![GPU Usage](local-ai-server/screenshots/08-gpu-usage.png)

Open WebUI is deployed using Docker and connects to a locally running Ollama

![Chat Test](local-ai-server/screenshots/07-chat-test.png)

Docker Running

![Docker Running](local-ai-server/screenshots/03-docker-running.png)

Open WebUI Container

![Open WebUI Container](local-ai-server/screenshots/04-openwebui-container.png)

Open WebUI Admin Setup

![Open WebUI Admin Setup](local-ai-server/screenshots/05-openwebui-admin.png)

Open WebUI chat

![Open WebUI Chat](local-ai-server/screenshots/06-openwebui-chat.png)





## Author

**Aarinnn**  
Computer Science / Data & Systems Projects  
GitHub: https://github.com/Aarinnn








