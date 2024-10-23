# GDSC Fall 2024 Workshop: Building an AI Chatbot with Spring AI, React, and Docker

## Introduction

Welcome! In this workshop, we will be building an AI chatbot application using Spring Boot, React, Docker, and OpenAI. 

## **Table of Contents**

1. [Overview](#overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Prerequisites](#prerequisites)
5. [Project Setup](#project-setup)
6. [Installing Dependencies](#installing-dependencies)
7. [Running the Application with Docker](#running-the-application-with-docker)
8. [Running Applications Locally (Without Docker)](#running-applications-locally-without-docker)
9. [API Endpoints](#api-endpoints)
10. [Customization](#customization)
11. [Deployment](#deployment)
12. [Conclusion](#conclusion)
13. [Acknowledgments](#acknowledgments)

### **Overview**

This project is a full-stack web application built with Spring Boot, React, and Docker. It serves as a learning tool for developers interested in integrating AI capabilities into their applications using the OpenAI API.

### **Features**

- **Interactive Chatbot**: Engage with a chatbot to explore Spring AI integration.
- **Spring Boot Backend**: Robust backend utilizing Spring AI for processing and generating responses.
- **React Frontend**: User-friendly interface for interacting with the chatbot.
- **Dockerized Setup**: Easy setup and deployment using Docker.

### **Tech Stack**

#### **Backend**

- **Java 17**  
  A high-level, class-based, object-oriented programming language that is widely used for building enterprise-scale applications.

- **Spring Boot**  
  An open-source Java-based framework used to create stand-alone, production-grade Spring-based applications with minimal configuration.

- **OpenAI API**  
  Provides access to powerful AI models that can perform tasks such as text generation, summarization, translation, and more.

#### **Frontend**

- **React**  
  A JavaScript library for building user interfaces, particularly single-page applications where data changes over time.

#### **DevOps**

- **Docker**  
  A platform used to develop, ship, and run applications inside containers, which are lightweight and portable execution environments.

Certainly! Here are the changes made to the **Prerequisites** section, including detailed installation instructions:

### **Prerequisites**

Ensure you have the following installed:

#### **Docker Installation**

1. Download Docker from the official website.
2. Follow the installation instructions specific to your operating system (Windows, macOS, or Linux).
3. Verify the installation by running:
   ```bash
   docker --version
   ```

#### **Docker Compose Installation**

1. Docker Compose is included with Docker Desktop on Windows and macOS.
2. For Linux, follow the instructions on the Docker Compose GitHub repository to install it separately.
3. Verify the installation by running:
   ```bash
   docker-compose --version
   ```

#### **Java 17 Installation**

1. Download Java 17 from the Oracle website or use an open-source alternative like OpenJDK.
2. Follow the installation instructions for your operating system.
3. Verify the installation by running:
   ```bash
   java -version
   ```

#### **Node.js and npm Installation**

1. Download Node.js from the official website (npm is included).
2. Follow the installation instructions for your operating system.
3. Verify the installation by running:
   ```bash
   node -v
   npm -v
   ```
   
### **Project Setup**

1. Fork the repository from GitHub to your account.
2. Clone your forked repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/REPO_NAME.git
   ```
3. Navigate into the cloned directory:
   ```bash
   cd REPO_NAME
   ```

### **Installing Dependencies**

#### Backend (Spring Boot)

1. Navigate to `spring-boot-ai-chatbot/`:
   ```bash
   cd spring-boot-ai-chatbot/
   ```
2. Create a `.env` file with your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key
   ```

#### Frontend (React)

1. Navigate to `chatbot-ui/`:
   ```bash
   cd chatbot-ui
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### **Running the Application with Docker**

1. Build and run the containers using Docker Compose:
   ```bash
   docker-compose up --build
   ```
2. Access the applications at:
   - Backend: `http://localhost:8080`
   - Frontend: `http://localhost:3000`

### **Running Applications Locally (Without Docker)**

#### Backend (Spring Boot)

1. Build and run:
   ```bash
   ./mvnw clean install spring-boot:run
   ```
2. Access the backend API at `http://localhost:8080`.

#### Frontend (React)

1. Start the React application:
   ```bash
   npm start
   ```
2. Access the frontend at `http://localhost:3000`.

### **API Endpoints**

- `GET /ai/chat/string`: Accepts a message query parameter and returns an AI-generated response.
  
- `POST /ai/chat`: Accepts a JSON body with a message field.

### **Customization**

#### Modifying the Frontend

Customize UI components in `src/` and styles in `Chatbot.css`.

#### Modifying the Backend

Modify services and controllers in `src/main/java`.

### **Deployment**

#### Docker Deployment on Local

Build Docker images using:
```bash
docker-compose build
```

#### Manual Deployment (Without Docker)

**Backend**: Deploy Spring Boot jar to a server or cloud service.

**Frontend**: Build React app (`npm run build`) and serve it with a web server.

### **Conclusion**

Congratulations! You have successfully set up an AI chatbot application using Spring Boot, React, Docker, and OpenAI.

Feel free to extend this project by adding features like user authentication, chat history persistence by integrating databases, and/or sentiment analysis!

### **Acknowledgments**

Thanks to FreeCodeCamp for providing the template to this workshop [here](https://www.freecodecamp.org/news/ai-chatbot-with-spring-react-docker/)!

You can visit the original project repo [here](https://github.com/vikasrajputin/springboot-react-docker-chatbot).
