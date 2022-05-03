# qb-ambulancejob 
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: hospital:server:SetArmor(amount) | 5/10
Issue: Set armor to any amount.

Solution: Server side only?

Notes: 


### NetEvent: hospital:server:RevivePlayer(playerId, isOldMan) | 5/10
Issue: Revive anyone from anywhere

Solution: Distance and item checks

Notes: 
