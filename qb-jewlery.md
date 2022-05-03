# qb-jewlery
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-jewellery:server:setVitrineState(stateType, state, k) | 7/10
Issue: Can remotely update state for any location

Solution: Needs more server side checks.

Notes: May be integral to system, may have to look into slight rework.

### NetEvent: qb-jewellery:server:vitrineReward | 10/10
Issue: Can be spammed for infinate rewards

Solution: Implement or utilize server side state management system and general server side checks.

Notes: 