# 🔑 SK-KEYS [REWORKED] 🔑

Advanced Vehicle Key & Lock System

Framework Compatible: QB-Core • QBOX • ESX
Inventory Compatible: ox_inventory • qb-inventory • qs-inventory

📌 Overview

SK-Keys is a secure, multi-framework vehicle key system designed for serious roleplay servers.

It supports:

Permanent vehicle keys

Temporary keys (admin / hotwire)

Key lock reset system

Key invalidation system (keylock)

Hotwire system

Lockpick system

Multi-dispatch support

Multi-target support

Discord webhook logging

Fully modular bridge system

Framework auto-detection

Inventory abstraction layer

🧠 How It Works

Each vehicle in the database has a keylock value.

When locks are changed:

The keylock value increases.

Old keys become invalid automatically.

Only keys with matching keylock work.

This prevents:

Key duplication exploits

Permanent stolen key abuse

Item cloning abuse

🔐 Security Model

Server-side ownership validation

No client trust

Key metadata verification

Spam protection

Framework abstraction

Inventory abstraction

Optional Discord logging

Debug mode for development

⚙ Configuration

Located in:

shared/shared.lua


Important options:

Shared.UseInventory = 'qs-inventory' -- qb-inventory / ox-inventory / qs-inventory
Shared.UseCommands = true
Shared.UseKeyLockSystemDatabase = true
Shared.SpawnMaxMods = true
Shared.Debug = false

🚘 Admin Commands
/car [model]

Spawns a vehicle with:

Max mods (if enabled)

Temporary key automatically assigned

/dv

Deletes current vehicle and removes temporary key.

🗝 Key System
Permanent Key

Given when:

Player buys a vehicle

Server manually gives key

Temporary Key

Given when:

Admin uses /car

Player hotwires vehicle

Temporary keys bypass DB ownership checks.

🔄 Supported Dispatch Systems

ps-dispatch

qs-dispatch

cd_dispatch

custom

Configured in:

Shared.Dispatch = 'ps'

🎯 Target Support

Automatically supports:

ox_target

qb-target

📡 Discord Webhook Logging

Supports:

Vehicle purchase logs

Lock change logs

Admin command logs

Configure:

Shared.Webhook = {
    Enabled = true,
    URL = "YOUR_WEBHOOK_URL",
    LogVehicleBuy = true,
    LogLockChanges = true,
    LogAdminCommands = true
}

🧩 Export Usage (Recommended)

⚠ Do NOT trigger server events directly.
Use exports instead.

🔑 Buy Vehicle (Give Permanent Key)
exports['sk-keys']:BuyVehicle(plate, model)


Example (vehicleshop):

exports['sk-keys']:BuyVehicle("ABC123", "sultan")

🗝 Give Temporary Key
exports['sk-keys']:givetemporary(plate)

❌ Remove Temporary Key
exports['sk-keys']:removetemporary(plate)

🔐 Change Locks
exports['sk-keys']:changelocks({
    plate = "ABC123"
})

🚗 Give Key Manually
exports['sk-keys']:givekeys(plate, model)

❌ Remove Permanent Key
exports['sk-keys']:removekey(plate)

📘 Example Integration
Vehicleshop Integration Example

Replace old vehicle key system:

-- REMOVE
-- TriggerEvent('vehiclekeys:client:SetOwner', plate)

-- ADD
exports['sk-keys']:BuyVehicle(plate, model)

🛠 Developer Mode

Enable debug:

Shared.Debug = true


You will see:

Framework detection

Ownership checks

Key metadata

Inventory operations

HasKey validation

Webhook status

Admin activity

Everything is modular and framework-independent.

🧠 Best Practices

✔ Always use exports
✔ Do not trigger events directly
✔ Keep Shared.Debug disabled in production
✔ Use Webhook logging for admin auditing
✔ Keep inventory item name consistent

💎 Premium Features

Key invalidation system

Multi-framework abstraction

Multi-inventory abstraction

Secure HasKey validation

Admin vehicle system

Temporary key system

Database lock reset

Optimized cache

Clean architecture ready for escrow

