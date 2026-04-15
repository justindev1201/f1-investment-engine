## Purpose
The purpose of this document is to record down the entities, their responsibilities and their relationships in the system.

## Main Entities
1. User
2. Room
3. RoomMember
4. Round
5. Driver
6. InvestmentEntry
7. RaceResult

## Responsibility of each entity
### User
Stores user identity and authentication-related information.

### Room
Stores room-level information such as room code and room metadata.

### RoomMember
Represents a user's membership in a room and their role in that room.

### Round
Stores round configuration and lifecycle state for a room.

### Driver
Stores driver reference data used for investments and results.

### InvestmentEntry
Stores one player’s investment amount for one driver in one round.

### RaceResult
Stores the podium result used to settle a round.

## Key relationships
1. One room can have many room members.
2. One user can belong to many rooms through room membership.
3. One room can have many rounds.
4. One round belongs to one room.
5. One round can have many investment entries.
6. One investment entry belongs to one user, one round, and one driver.
7. One user can have multiple investment entries in one round, but only one entry per driver.
8. One round has one race result record.
9. One race result belongs to one round.

## Business Rules
1. In one round, a player may invest in one or more drivers.
2. In one round, a player may only invest once per driver
3. The total of player's investment entries must use the full round budget.
4. A driver's total investment in a round must not exceed the configured pool cap.
5. Each round is settled using one associated race result record.
