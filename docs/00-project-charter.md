# F1 Investment Engine

## Goal
The goal of this project is to build an internal game for people who wants to add excitement and ability to customise while watching the F1 competition. 

## Target Users
The targeted users are people who wants to add little bit of excitement for their own purpose for f1 competition, e.g. friends and family, rather than outsourcing other bets.

## Problem Statement
How might we bring excitement and transparent calculations of bets for multiple users when betting on limited f1 drivers in the competition?

## Success Criteria
1. Users can complete a full game round from room creation to payout without errors
2. Payout calculations strictly match the defined mathematical rules
3. Invalid investments (e.g. exceeding pool cap, not using full budget) are rejected by the system
4. At least one full test round is successfully completed with real users 
5. The system is deployed and accessible online for testing

## Timeline
1. Define project and setup with MVP (end of Apr)
2. System tested and rectified (end of May)
3. Everything is polished with proper documentation (end of June)

## Scope
### Phase 1 - MVP
1. User registration and login
2. Create and join a game room via share code
3. Configure round rules such as starting budget and pool cap
4. Manage round lifecycle (open → locked → result → payout)
5. Allow players to allocate their full budget across drivers
6. Validate investment rules and lock submissions
7. Input actual race results for podium positions
8. Calculate payouts and jackpot outcomes correctly
9. Show round results and updated balances
10. Deploy a usable test version for small group testing

## Out of Scope - For MVP
1. Friends system or social relationships between users
2. Real-time chat or communication features
3. Detailed race data or external F1 API integration
4. Advanced UI/UX or polished design
5. Full account management features (e.g. profile editing, password reset)
6. Real-time updates (e.g. live syncing with websockets)
7. Scalability considerations for large number of users