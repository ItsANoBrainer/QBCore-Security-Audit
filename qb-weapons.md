# qb-weapons
General distance checks, item checks, and other basic security checks should be done on all net server events.

## server/main.lua

### NetEvent: weapons:server:AddWeaponAmmo(CurrentWeaponData, amount) | 7/10
Issue: Can set ammo of weapon to anything

Solution: Server side verification checks

Notes: 

### NetEvent: weapons:server:UpdateWeaponAmmo(CurrentWeaponData, amount) | 7/10
Issue: Can set ammo of weapon to anything

Solution: Server side verification checks

Notes: 

### NetEvent: weapons:server:SetWeaponQuality(data, hp) | 7/10
Issue: Can set quality of weapon to anything

Solution: Server side verification checks

Notes: 