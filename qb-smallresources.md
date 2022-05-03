# qb-smallresources
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/logs.lua

### NetEvent: qb-log:server:CreateLog(name, title, color, message, tagEveryone) | 5/10
Issue: Can trigger and spam logs from client side

Solution: Make server side only

Notes: 
