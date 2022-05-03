# qb-policejob
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: police:server:TakeOutImpound(plate) | 3/10
Issue: Remove any plate out of impound

Solution: Job/distance checks?

Notes: 


### NetEvent: police:server:SeizeCash, function(playerId) | 7/10
Issue: Take anyones money

Solution: Job/distance checks?

Notes: 


### NetEvent: police:server:SeizeDriverLicense, function(playerId) | 7/10
Issue: Remove anyones license

Solution: Job/distance checks?

Notes: 


### NetEvent: police:server:RobPlayer, function(playerId) | 7/10
Issue: Take anyones money

Solution: Job/distance checks?

Notes: 
