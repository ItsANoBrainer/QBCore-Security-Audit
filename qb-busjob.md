# qb-busjob
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: qb-busjob:server:NpcPay(Payment) | 10/10
Issue: Can give self as much money as you want

Solution: Save drive states server side?

Notes: Has some basic distance and job checking, but really not enough.
