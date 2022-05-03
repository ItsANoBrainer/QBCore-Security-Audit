# qb-vehiclesales
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-occasions:server:sellVehicleBack', function(vehData) | 10/10
Issue: Infinite money generation

Solution: Server side verifications

Notes: 
```lua
TriggerServerEvent('qb-occasions:server:sellVehicleBack', { model = `asbo`} )
```