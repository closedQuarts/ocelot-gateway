
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
