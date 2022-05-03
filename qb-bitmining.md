# qb-bitmining
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server.lua

### NetEvent: qb-cryptomining:server:addCryptoCoinsfunction(reward) | 10/10
Issue: Can pass any reward amount to add any amount of crypto currency

Solution: Handle this server side state.

Notes: 

### NetEvent: qb-cryptomining:server:RemoveItem(item) | 3/10
Issue: Can remove any item from self inventory

Solution: Only allow removal of specific item instead of paramter passing.

Notes: 