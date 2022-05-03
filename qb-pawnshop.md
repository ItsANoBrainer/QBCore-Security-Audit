# qb-pawnshop
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-pawnshop:server:pickupMelted(item) | 10/10
Issue: Can spawn any items you want

Solution: Save items being melted server side as they get removed from inventory

Notes:

Example: 
```lua
TriggerServerEvent('qb-pawnshop:server:pickupMelted', {
    ["items"] = {
        {
            ["item"] = {["reward"] = {{["item"] = "meth", ["amount"] = 100}}},
            ["amount"] = 1
        }
    }
})
```
