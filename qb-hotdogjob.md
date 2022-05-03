# qb-hotdogjob
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-hotdogjob:server:Sell(Amount, Price) | 10/10
Issue: Can pass any amount to give that much money.

Solution: Basic server side checks and amout clamps. 

Notes: Could also implement system to only allow a certain number of triggers in a timeframe.