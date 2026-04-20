# Development Environment Setup

## Purpose
This document defines the development environment setup and project structure to ensure consistent local development and smooth onboarding of tools before implementation begins.

## Planned Project Structure
/backend
/frontend
/docs

## Required Tools
- Git
- .NET SDK
- Node.js
- PostgreSQL
- Visual Studio 2026 Community (recommended for backend)
- VS Code (recommended for frontend, docs, and general editing)
- Postman

## Backend Setup Plan
- Use ASP.NET Core Web API
- Located inside /backend
- Handles business logic, validation, and API endpoints

## Frontend Setup Plan
- Use React for UI
- Located inside /frontend
- Handles user interaction and API communication

## Local Development Plan
- Backend runs on localhost:5000
- Frontend runs on localhost:3000
- Frontend sends HTTP requests to backend API
- Backend connects to local PostgreSQL database