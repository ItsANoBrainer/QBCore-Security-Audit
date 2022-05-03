# qb-houserobbery
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-houserobbery:server:SetBusyState(cabin, house, bool) | 7/10
Issue: Can remotely update state for any location

Solution: Needs more server side checks.

Notes: May be integral to system, may have to look into slight rework.

### NetEvent: qb-houserobbery:server:searchCabin(cabin, house) | 10/10
Issue: Can be spammed for rewards. Does not use server side state system server side.

Solution: Do checks server side on the state system that was implemented.

Notes: 