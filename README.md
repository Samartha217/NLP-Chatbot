# NLP-Chatbot

Here’s a rephrased version of the README file, including a brief introduction:

---

## Introduction

A chatbot is an AI-driven software application designed to interact with users through text or voice. Chatbots are commonly used in customer service, information retrieval, and task automation, making them valuable tools in various industries. This project focuses on creating an NLP (Natural Language Processing) chatbot using Python, FastAPI, and Dialogflow, integrated with a MySQL database for data management.

## Project Structure

- **backend**: This directory contains the FastAPI-based backend code for the chatbot.
- **db**: Contains the MySQL database dump, which should be imported into your MySQL database using a tool like MySQL Workbench.
- **dialogflow_assets**: Holds training phrases and other assets for Dialogflow intents.
- **frontend**: Contains the code for the website interface.

## Installation Instructions

To set up the environment, you can install the required modules individually or all at once:

- Install modules separately:
  ```bash
  pip install mysql-connector
  pip install "fastapi[all]"
  ```

- Alternatively, you can install all dependencies at once by running:
  ```bash
  pip install -r backend/requirements.txt
  ```

## Running the FastAPI Backend Server

1. Navigate to the `backend` directory using your command prompt.
2. Start the server by executing the following command:
   ```bash
   uvicorn main:app --reload
   ```

## Setting Up Ngrok for HTTPS Tunneling

1. Download the appropriate Ngrok version for your operating system from [Ngrok's official website](https://ngrok.com/download).
2. Extract the downloaded zip file and place `ngrok.exe` in a folder of your choice.
3. Open the Windows command prompt, navigate to that folder, and run:
   ```bash
   ngrok http 8000
   ```

   **Note**: Ngrok sessions can time out. If you encounter a "session expired" message, you'll need to restart the session.

---
