# qb-storerobbery
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-storerobbery:server:takeMoney(register, isDone) | 8/10
Issue: Trigger acquiring reward for robbery.

Solution: Server side register hittable states and more checks. (distance/etc.)

Notes: 


### NetEvent: qb-storerobbery:server:setRegisterStatus(register) | 5/10
Issue: Reset register status. When combined with other triggers unlimited money.

Solution: Make server side only

Notes: 


### NetEvent: qb-storerobbery:server:setSafeStatus(safe) | 5/10
Issue: Reset register status. When combined with other triggers unlimited money.

Solution: Make server side only

Notes: 


### NetEvent: qb-storerobbery:server:SafeReward(safe) | 8/10
Issue: Trigger acquiring reward for safe.

Solution: Server side register hittable states and more checks. (distance/etc.)

Notes: 
