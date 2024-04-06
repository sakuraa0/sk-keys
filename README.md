# 🔑 sk-keys [v.1.2] 🔑

Sk-keys Script for qb-core 
author: Sakura Scripts

Buy Now: https://sk-scripts-webstore.tebex.io/package/6179402 
Docs: [https://app.gitbook.com/o/kTlCKAoKMU0nfhJuQKn5/s/OyepVcY3QAsjRL5pHyIV/](https://sakura-scripts.gitbook.io/sakura-script-key/)
Preview: (https://www.youtube.com/watch?v=wXjW2OduMJs)
Discord: https://discord.gg/HCaADtSrYt


Read:

##export to remove temporary key
exports['sk-keys']:removetempkey(plate)

##export to remove key 
exports['sk-keys']:removekey(plate)

##export for testdrive 
exports['sk-keys']:givetemporary(plate)

##export to buy
exports['sk-keys']:buyvehicle(plate, model)

##give robbed key 
exports['sk-keys']:changelocks(plate)

##Change Car locks
exports['sk-keys']tempkey(data)

##Give Keys (Garage, jobs and more)
exports['sk-keys']givekey(plate, model)

items:

vehiclekey                   = { name = 'vehiclekey', label = 'Vehicle key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
robbedvehkey                   = { name = 'robbedvehkey', label = 'Robbed Key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
neonkit                   = { name = 'neonkit', label = 'Neon Key', weight = 10, type = 'item', image = 'neonkit.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "Turn on/off your neons" },


Dependencies:

UI FOR MINIGAMES HACK: (You can change in utils.lua)

https://github.com/Project-Sloth/ps-ui

Disptach (Soon ill be changeable)

https://github.com/Project-Sloth/ps-dispatch

Lockpick: (you can change it to)

https://github.com/sakuraa0/Lockpick-FiveM-qb-esx

