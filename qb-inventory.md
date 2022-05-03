# qb-inventory
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: inventory:server:addTrunkItems(plate, items) | 10/10
Issue: Set any plate trunk to any items you want

Solution: Make server side only

Notes: 


### NetEvent: inventory:server:CraftItems(itemName, itemCosts, amount, toSlot, points) | 10/10
Issue: Can remove and add item items you want

Solution: Verify the player has the items???

Notes: 
```lua
TriggerServerEvent('inventory:server:CraftItems', "meth", {}, 5, 5, 5)
```


### NetEvent: inventory:server:CraftAttachment(itemName, itemCosts, amount, toSlot, points) | 10/10
Issue: Can remove and add item items you want

Solution: Verify the player has the items???

Notes: 
```lua
TriggerServerEvent('inventory:server:CraftItems', "meth", {}, 5, 5, 5)
```


### NetEvent: inventory:server:OpenInventory(name, id, other) | 10/10
Issue: Can open any inventory. Most important would be OTHERPLAYER and SHOP. Can create a shop with
any items and any price.

Solution: Distance check or anything.

Notes: 
```lua
TriggerServerEvent('inventory:server:OpenInventory', "otherplayer", 1)
```


### NetEvent: qb-inventory:server:SaveStashItems(stashId, items) | 10/10
Issue: Set items to any stash

Solution: Make server side only, verify items.

Notes: 
