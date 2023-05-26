# AI Teaching Assistant

Use at https://whyth.app or deploy your own. 

***

## Overview

Powered by OpenAI API, this app brings an educational wrapper over ChatGPT you know so well.

But wait, it's more what just a wrapper, it also can limit AI in a lot of ways. (WIP)

It also can use your own material to teach and answer questions (Coming Soon)

### Key Features
#### 1. Custom Lesson Creation for Teachers
* Teachers can create lessons by entering a subject/topic and a brief description or outline.
* (WIP) Also, limit the usage of AI by the students (for example: not give out answers to the problems, or don't talk about specific topics)
* (WIP) Teachers can use their own to enhance the AI's knowledge base.
#### 2. Easy Lesson Joining for Students
* Students can join lessons using a unique lessonID or a link provided by their teacher.
* The AI uses the provided subject/topic and any additional resources to generate contextually relevant responses.
#### 3. AI-Driven Chat for Interactive Learning
* Students can interact with the AI chat assistant to ask questions, discuss concepts, or request explanations.
* The AI provides answers, clarifications, and examples based on the subject/topic and any additional resources supplied by the teacher.


## Development setup

First of all, update subomdules:

```
git submodule update --remote --recursive
```

### Backend

>Note: You need **redis-server** running on your machine

1. Create `.env` 
2. Set `API_KEY` environrment variable
2. Run `main.go`

Refer to `.env.example` and `config.go` for the complete list of env variables.
  
### Frontend

1. `npm install`
2. Uncomment `setupProxy.js` (for CORS issues)
3. `npm start`

## Roadmap

### Work in progress
- [x] Use system message to limit AI responses
- [x] Teacher can configure the AI's behaviour (several options to map to system message)
- [ ] Teacher can Upload PDF files for AI to use as reference (use langchain)
 
### Needs to be done

1. Chat markdown formatting
2. Chat prompt suggestions
3. Stream AI response instead of loader
4. Responsive UI for mobile devices
5. Fine-tuning the model to deliver clear & concise responses

### Possible features

1. Lesson management for a teacher & multiple lessons
2. *AI can Represent graphs & formulas (for math & physics)*
3. Multiple chat sessions (to be able to switch between them)
4. Custom lesson timeouts
5. Responsive UI for mobile devices
6. Mobile app
