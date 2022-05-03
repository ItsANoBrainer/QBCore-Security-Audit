# qb-bankrobbery
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-bankrobbery:server:setBankState(bankId, state) | 3/10
Issue: Can reset any bank at any time.

Solution: Make server side only.

Notes: 


### NetEvent: qb-bankrobbery:server:setLockerState(bankId, lockerId, state, bool) | 7/10
Issue: Can reset any bank locker at any time.

Solution: Make server side only.

Notes: 


### NetEvent: qb-bankrobbery:server:recieveItem(type) | 10/10
Issue: Can trigger item receiving from any bank.

Solution: Make server side only. Add more checks to if the locations are even hittable. Have a server state for each location.

Notes: 
