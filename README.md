# 🔑 sk-keys [v.1.2] 🔑

Sk-keys Script for qb-core 
author: Sakura Scripts

Buy Now: https://sk-scripts-webstore.tebex.io/package/6179402 


Docs: [https://app.gitbook.com/o/kTlCKAoKMU0nfhJuQKn5/s/OyepVcY3QAsjRL5pHyIV/](https://sakura-scripts.gitbook.io/sakura-script-key/)


Preview: (https://www.youtube.com/watch?v=wXjW2OduMJs)


Discord: https://discord.gg/HCaADtSrYt


Read:

##export to remove temp key
exports['sk-keys']:removetempkey(plate)

##Remove Temporary Key item 
exports['sk-keys']:removetemporary(plate)

##export to remove key 
exports['sk-keys']:removekey(plate)

##Temporay key
exports['sk-keys']:givetemporary(plate)

##export to buy
exports['sk-keys']:buyvehicle(plate, model)

##Change lock key
exports['sk-keys']:changelocks(plate)

##Temporary Key
exports['sk-keys']:tempkey(data)

##Give Keys
exports['sk-keys']:givekey(plate, model)

items:

vehiclekey                   = { name = 'vehiclekey', label = 'Vehicle key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
robbedvehkey                   = { name = 'robbedvehkey', label = 'Robbed Key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
neonkit                   = { name = 'neonkit', label = 'Neon Key', weight = 10, type = 'item', image = 'neonkit.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "Turn on/off your neons" },


Dependencies:

UI FOR MINIGAMES HACK: (You can change in utils.lua)

https://github.com/Project-Sloth/ps-ui

Disptach (You can change in utils.lua)

https://github.com/Project-Sloth/ps-dispatch

Lockpick: (You can change in utils.lua)

https://github.com/sakuraa0/Lockpick-FiveM-qb-esx

