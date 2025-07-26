# Mastra Assistant UI Template

This project demonstrates a full-stack chat application using Mastra for the backend and assistant-ui for the frontend.

## Prerequisites

- Node.js >= v22.0.0
- OpenAI API key

## Setup

1. **Configure Environment Variables**

   Copy the example environment file and add your OpenAI API key:
   ```bash
   cp backend/.env.example backend/.env
   ```

   Then edit `backend/.env` and replace the placeholder with your actual OpenAI API key:
   ```
   OPENAI_API_KEY=sk-proj-YOUR_ACTUAL_API_KEY_HERE
   ```

2. **Install Dependencies**

   From the root directory:
   ```bash
   npm install
   ```

## Running the Application

1. **Start Both Backend and Frontend**

   From the root directory:
   ```bash
   npm run dev
   ```

   This will start:
   - Backend on http://localhost:4111
   - Frontend on http://localhost:3000

2. **Access the Application**

   Open your browser and navigate to http://localhost:3000

## Available Scripts

From the root directory:

- `npm run dev` - Start both backend and frontend in development mode
- `npm run dev:backend` - Start only the backend
- `npm run dev:frontend` - Start only the frontend
- `npm run build` - Build both applications
- `npm run start` - Start both applications in production mode

## Project Structure

```
mastra-assistant-ui-template/
├── backend/              # Mastra backend
│   ├── src/
│   │   └── mastra/
│   │       ├── agents/   # AI agents
│   │       ├── tools/    # Tools including MCP client
│   │       └── workflows/
│   └── .env             # Backend environment variables
├── frontend/            # Assistant UI frontend
│   └── app/
│       └── assistant.tsx # Main chat component
└── README.md
```

## Features

- Mastra backend with tool using Weather agent
- Assistant-UI frontend with streaming chat

## Next Steps

- Add authentication
- Implement additional MCP or additional tools
- Customize the UI theme and branding
