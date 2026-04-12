# Initial Tech Stack Decision

## Purpose
The purpose of this document is to record the tech stack chosen and rationale for this project

## Requirements
- Support a full-stack web application
- Strong backend support for business logic
- Easy to develop and maintain as a solo developer
- Simple deployment process
- Good learning value for backend and system design
- Stable ecosystem and documentation
- Reasonable performance for small-scale usage

## Candidate Options

### Option A: C# / ASP.NET Core + React + PostgreSQL
- Backend: ASP.NET Core Web API
- Frontend: React
- Database: PostgreSQL

### Option B: TypeScript / Node.js + React + PostgreSQL
- Backend: Node.js with TypeScript
- Frontend: React
- Database: PostgreSQL

### Option C: Next.js + PostgreSQL
- Full-stack: Next.js
- Database: PostgreSQL

## Proposed Stack
- Backend: C# with ASP.NET Core Web API
- Frontend: React
- Database: PostgreSQL

## Rationale
1. This stack has the strongest learning leverage from my current background in C#.
2. ASP.NET Core is well-suited for backend-heavy business logic and API development.
3. React is a practical frontend choice with a large ecosystem and clear separation from backend concerns.
4. PostgreSQL is widely used, stable, and suitable for relational data such as users, rooms, rounds, and investments.
5. This stack supports a clean full-stack architecture without introducing unnecessary complexity for a solo project.

## Risks / Tradeoffs
1. Using React and ASP.NET Core means working across two separate application layers, which increases setup and integration complexity compared to a single full-stack framework.
2. PostgreSQL is new to me compared to databases I have used before, so there may be an initial learning curve.
3. This stack may require more setup effort at the beginning before feature development can move quickly.
4. Frontend and backend deployment may need to be managed separately depending on hosting choice.

## Open Questions
1. Which React project setup should be used for the frontend?
2. Which ORM or database access approach should be used in ASP.NET Core?
3. Which authentication approach should be used for MVP?
4. Where should the application be hosted for testing and deployment?
5. Should frontend and backend be deployed together or separately?