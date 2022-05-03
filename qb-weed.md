# qb-weed
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-weed:server:placePlant(coords, sort, currentHouse) | 5/10
Issue: User can place as many plants as they want with no item verification

Solution: Item verification and other general server side checks.

Notes: 