# qb-vehiclefailure
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server.lua

### NetEvent: qb-vehiclefailure:removeItem(item) | 3/10
Issue: Remove any item from self

Solution: Make the event only remove a certain item

Notes: 
