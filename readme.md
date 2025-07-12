Credit to hhfw1
Original Repo found [here](https://github.com/hhfw1/hh_aidoc).

Functions:
- Adds QB-Core AI EMS/Medic
- Fixes/Bypasses QB-Core ban for reviving through client side

Installation
Head into QB-Ambulance Job/server/main.lua and add this function: 

```
-- AIMedic Function (HH AI EMS)
RegisterNetEvent('hospital:server:ForceRevive', function()
    local src = source
    TriggerClientEvent('hospital:client:Revive', src)
end)
```