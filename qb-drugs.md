# qb-drugs
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/cornerselling.lua

### NetEvent: qb-drugs:server:sellCornerDrugs(item, amount, price) | 10/10
Issue: Can sell any item in any amount for any price instantly

Solution: Have list of sellable items server side, more server side checks/verifications. Not trust client sent
parameters.

Notes: 

## server/deliveries.lua

### NetEvent: qb-drugs:server:CreateDealer(DealerData) | 10/10
Issue: Can create dealer with any data

Solution: Add permission or server side checks. Don't trust client blindly.

Notes: 

### NetEvent: qb-drugs:server:updateDealerItems(itemData, amount, dealer) | 10/10
Issue: Can be used to give any cash amount passed

Solution: Dont trust client data

Notes: 

### NetEvent: qb-drugs:server:giveDeliveryItems(amount) | 5/10
Issue: Gives player any amount of weed bricks

Solution: Server side verification checks, dont trust amount sent by client.

Notes: Escalates to 10/10 issue rating when used with `qb-drugs:server:succesDelivery`

### NetEvent: qb-drugs:server:giveDeliveryItems(amount) | 10/10
Issue: Redeem any amount of cash for all weed bricks. Can be used with `qb-drugs:server:giveDeliveryItems`.

Solution: Server side verification checks, dont trust amount sent by client.

Notes: 
