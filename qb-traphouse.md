# qb-traphouse
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-traphouse:server:RobNpc(Traphouse) | 10/10
Issue: Infinite money and passcode generation for traphouse

Solution: Server side verifications

Notes: 

### NetEvent: qb-traphouse:server:AddHouseKeyHolder', function(CitizenId, TraphouseId, IsOwner) | 5/10
Issue: Ability to overwrite traphouse keyholder and pincode if IsOwner is passed as true

Solution: Server side checks for actual ownership or key having

Notes: 