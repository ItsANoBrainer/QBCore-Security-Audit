# qb-houses
General distance checks, item checks, and other basic security checks should be done on all net server events.
Entire resource needs realtor job checks.

## server/main.lua

### NetEvent: qb-houses:server:createBlip | 1/10
Issue: Create unowned house blip at current location to all players

Solution: Job check

Notes: 


### NetEvent: qb-houses:server:addNewHouse(street, coords, price, tier) | 5/10
Issue: Create a house for any amount anywhere.

Solution: Job check

Notes: 


### NetEvent: qb-houses:server:addGarage(house, coords) | 5/10
Issue: Create a garage for any amount anywhere.

Solution: Job check

Notes: 
