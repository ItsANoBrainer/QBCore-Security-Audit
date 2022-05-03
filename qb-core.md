# qb-core
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/events.lua

### NetEvent: QBCore:Server:SetMetaData(meta, data) | 3/10
Issue: Can set any metadata of self to anything.

Solution: This should probably be a server only event.

Notes: 


### NetEvent: QBCore:Server:UseItem(item) | 10/10
Issue: Can remotely trigger use any item without having it in inventory.

Solution: Verify user has the item instead of blindly trusting parameters.

Notes: Item parameter only needs to be this this:
Example: 
```lua
TriggerServerEvent('QBCore:Server:UseItem', { ["name"]="meth", ["amount"]=100, })
```


### NetEvent: QBCore:Server:RemoveItem(itemName, amount, slot) | 3/10
Issue: Can remove any item from self

Solution: Remove or make server side only

Notes: 


### NetEvent: QBCore:Server:AddItem(itemName, amount, slot, info) | 10/10
Issue: Can add any item to self

Solution: Remove or make server side only

Notes: PR to fix all instances of this already exists.
