# sk-keys
Sk-keys Script for qb-core

Buy Now: https://sk-scripts-webstore.tebex.io/package/6179402 

Docs: https://app.gitbook.com/o/kTlCKAoKMU0nfhJuQKn5/s/OyepVcY3QAsjRL5pHyIV/

Usefull Readme

##export to give key
exports['sk-keys']:givekey(plate, model)
##export to remove key 
exports['sk-keys']:removekey(plate)
##export for testdrive 
exports['sk-keys']:testdrive(plate)
##export to buy
exports['sk-keys']:buyvehicle(plate, model)
##give robbed key 
exports['sk-keys']:givetemporarykey(plate)
##Change Car locks
exports['sk-keys']changelocks(data)

items:

vehiclekey                   = { name = 'vehiclekey', label = 'Vehicle key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
robbedvehkey                   = { name = 'robbedvehkey', label = 'Robbed Key', weight = 10, type = 'item', image = 'vehiclekeys.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "" },
neonkit                   = { name = 'neonkit', label = 'Neon Key', weight = 10, type = 'item', image = 'neonkit.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = "Turn on/off your neons" },
