# Ocelot API Gateway

This repository contains the Ocelot API Gateway configuration used to route all chat-related backend API requests. The gateway is hosted on Render and handles routing to .NET-based billing services.

## Features

- Handles requests for:
  - /api/bill/{subscriberId}
  - /api/bill/detailed
  - /api/bill/pay
- Configured using Ocelot (ocelot.json)
- Hosted on Render
- Uses JWT token validation where needed

## Related Repositories

Frontend UI: ai-chat-ui  
Firebase Function: firabase-chat-agent

## Developer

Name: Efe Demirtaş  
Course: SE4458 Software Architecture (Spring 2025)  
Project: AI Chat Agent (Gateway)

## Challenges Encountered

- Coordinating communication between the React frontend, Firebase functions, and the Ocelot API Gateway required precise endpoint and method alignment.
- Managing CORS and authorization headers when calling the gateway from cloud functions.
- Parsing natural language reliably using OpenAI and designing consistent JSON outputs for varying user intents.
- Handling asynchronous behavior between Firestore message writes and delayed function triggers.
- Configuring Firebase project permissions to allow the frontend to write and read from Firestore.
- Debugging unexpected 401 and 404 errors from the gateway during early integration.

[Youtube](https://www.youtube.com/watch?v=t0SbUoxAgKk)
[ai-chat-ui](https://github.com/closedQuarts/ai-chat-ui)
[firabase-chat-agent](https://github.com/closedQuarts/firabase-chat-agent)
