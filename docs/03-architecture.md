# Initial Architecture Direction

## Purpose
The purpose of this document is to give a clear direction of what are the major parts the system needs, how they interact, where the main responsibilities live and what are we deliberately keeping simple for MVP.

## System Type
This is a full-stack web application that would be deployed online and targets small groups of F1 fans. Its logic is driven by a room-based multiplayer game application.

## High-Level Components
1. Frontend client
2. Backend application
3. Authentication module
4. Room and round management module
5. Investment validation module
6. Payout and jackpot calculation module
7. Database
8. Deployment and infrastructure

## Responsibilities of Each Component
### Frontend
1. Collect user input
2. Display room, round, and payout information
3. Sned requests to backend API
4. Show validation errors and round results

### Backend API
1. Expose API endpoints
2. Handle requests and responses
3. Coordinate business logic across modules
4. Communicate with the database
5. Enforce server-side validation

### Authentication module
1. Register user
2. Authenticate login requests
3. Manage user identity and access control

### Room & Round management
1. Create and join private rooms
2. Generate and validate share codes
3. Configure game round settings
4. Manage round lifecycle states such as open, locked, and settled

### Investment validation module
1. Accept player investment submissions
2. Validate full budget usage
3. Enforce pool cap rules
4. Prevent invalid actions where required

### Payout and jackpot calculation module
1. Process podium results
2. Calculate payouts according to documented rules
3. Handle case where no one wins certain positions
4. Carry forward jackpot when required

### Database
1. Store users, rooms, rounds, investments, results, and balances
2. Persist system state between sessions
3. Support retrieval of data for game display and settlement

### Deployment and infrastructure
1. Host the application
2. Provide environment configuration
3. Support deployed access for real user testing

## Core Data Flow
1. User registers or logs in
2. User creates or joins a private room
3. Room admin configures the round
4. Players submit investments
5. System validates each investment submission against game rules
6. Round is locked when submissions are complete or closed by the room admin
7. Room admin enters podium results
8. System calculates payouts and jackpot outcomes
9. Round results and updated balances are shown to users

## MVP Architecture Constraints
1. Monolithic architecture first, not microservices
2. Standard request-response web architecture for MVP
3. No real-time chat or live communication features
4. No live F1 API integration
5. No advanced scalability design for MVP-scale usage

## Open Questions
1. Tech stack is not finalized
2. Authentication approach is not finalized
3. Deployment approach is not finalized
