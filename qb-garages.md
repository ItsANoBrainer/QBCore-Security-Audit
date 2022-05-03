# qb-garages
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-garage:server:updateVehicle(state, fuel, engine, body, plate, garage) | 10/10
Issue: Ability to update the parameters directly to the database for any vehicle. Theoretically could brick anyones
vehicles in the database by setting state or garage to unknown variables.

Solution: Needs some kind of ownership only scope or moving this to a server side function. Some investigation
needs to be done to see if this is used by non owners to update the vehicle, and just rework this implementation
entirely. 

Notes: Check if server side natives exist for getting this information.

### NetEvent: qb-garage:server:updateVehicleState(state, plate, garage) | 10/10
Issue: Ability to update the parameters directly to the database for any vehicle. Theoretically could brick anyones
vehicles in the database by setting state or garage to unknown variables.

Solution: Needs some kind of ownership only scope or moving this to a server side function. Some investigation
needs to be done to see if this is used by non owners to update the vehicle, and just rework this implementation
entirely. 

Notes: Check if server side natives exist for getting this information.

