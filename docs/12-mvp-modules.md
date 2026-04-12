## Purpose
The purpose of this document is to define a clear plan of what the MVP would include and not include so that we ensure we don't over do the MVP.

## List of MVP modules
1. Authentication
2. Room Management
3. Round Management
4. Investment 
5. Payout and jackpot calculation module

## Responsibility of each module
### Authentication module
1. Register user
2. Authenticate login requests
3. Manage user identity and access control

### Room Module
1. Create and join private rooms
2. Generate and validate share codes for the room
3. Track room membership
4. Identify room admin permissions

### Round Module
1. Configure round settings such as starting budget and pool cap
2. Manage round lifecycle states such as open, locked, and settled
3. Determine and store player turn order for the round

### Investment module
1. Accept player investment submissions
2. Validate full budget usage
3. Enforce pool cap rules
4. Prevent invalid actions where required
5. Store submitted investments

### Payout and jackpot calculation module
1. Process podium results
2. Calculate payouts according to documented rules
3. Handle case where no one wins certain positions
4. Carry forward jackpot when required

## Module interactions
### Authentication
Provides user identity to all protected actions.

### Room Management
Uses authenticated users to create rooms, join rooms, and determine room membership and room admin.

### Round Management
Belongs to a room and controls the lifecycle and settings of each game round.

### Investment
Belongs to a round and uses round settings and user identity to validate and store investments.

### Payout and Jackpot Calculation
Uses round results and investment data to calculate payouts and update balances.

## What is intentionally exculeded for MVP
1. Friends system
2. Real-time chat
3. Live F1 API integration
4. Full account management features such as profile editing and password reset
5. Manual payment confirmation workflow inside the platform
6. Advanced analytics or race statistics