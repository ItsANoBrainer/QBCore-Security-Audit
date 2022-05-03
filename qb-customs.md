# qb-customs
General distance checks, item checks, and other basic security checks should be done on all net server events.

## qb-customs

### NetEvent: qb-customs:server:updateRepairCost(cost) | 3/10
Issue: Users can get free repair costs

Solution: Use natives server side (if possible) to generate this cost server side. Otherwise it may be impossible and
the client may have to be trusted with the repair cost amount it sends over.

Notes: Not very game breaking, but still an exploit regardless.