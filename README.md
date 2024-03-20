# 🔑 sk-keys [v.1.0.9] 🔑

Sk-keys Script for qb-core 
author: Sakura Scripts

Buy Now: https://sk-scripts-webstore.tebex.io/package/6179402 
Docs: https://app.gitbook.com/o/kTlCKAoKMU0nfhJuQKn5/s/OyepVcY3QAsjRL5pHyIV/
Preview: (https://www.youtube.com/watch?v=wXjW2OduMJs)
Discord: https://discord.gg/HCaADtSrYt


Read:

##export to give key
exports['sk-keys']:givekey(plate, model)
##export to remove key 
exports['sk-keys']:removekey(plate)
##export for testdrive 
exports['sk-keys']:tempkey(plate)
##export to buy
exports['sk-keys']:buyvehicle(plate, model)
##give robbed key 
exports['sk-keys']:robkey(plate)
##Change Car locks
exports['sk-keys']changelocks(data)

items:

vehiclekey                   = { name = 'vehiclekey', label = 'Vehicle key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
robbedvehkey                   = { name = 'robbedvehkey', label = 'Robbed Key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
neonkit                   = { name = 'neonkit', label = 'Neon Key', weight = 10, type = 'item', image = 'neonkit.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "Turn on/off your neons" },
