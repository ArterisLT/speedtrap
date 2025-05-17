# 🚓 FiveM Speed Trap Script

This is a lightweight FiveM script that creates **Speed Trap Zones** similar to those found in racing games like *Forza Horizon* or *Need for Speed*. Players must reach or exceed a specific speed inside the trap zone to trigger a notification and track their speed.

✨ Features

- Define multiple speed trap zones using coordinates and radius.
- Set individual speed requirements per trap (e.g., 200 km/h).
- Displays player's top speed when entering the trap zone.
- Fully client-sided and easy to configure.
- No database or SQL required.

🔧 Configuration

You can define your speed trap zones in `client.lua`:

```lua
local speedTraps = {
    {
        coords = vector3(208.13, 6556.76, 31.91),
        radius = 20.0,
        requiredSpeed = 200.0
    },
    {
        coords = vector3(-75.43, -818.36, 326.18),
        radius = 25.0,
        requiredSpeed = 180.0
    },
    -- Add more zones here
}
