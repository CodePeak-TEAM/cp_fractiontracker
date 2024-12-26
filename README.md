```markdown
# Factions Tracker

This project is a Lua script for tracking faction vehicles in a game. It creates blips on the map for vehicles belonging to specific factions.

## Features

- Tracks vehicles belonging to specified factions.
- Creates blips on the map for tracked vehicles.
- Updates blips periodically.
- Removes blips for vehicles that no longer exist.

## Configuration

The configuration for the script is located in the `config.lua` file.

### Factions

Specify the factions that should have blips:

```lua
Config.frakcje = {
    'police',
    'lssd',
    'ambulance',
}
```

### Faction Vehicles

Specify the list of vehicles for each faction:

```lua
Config.frakcjeAuta = {
    police = {
        'police',
        'police1',
        'police3'
    },
    lssd = {
        'sheriff',
        'sheriff1'
    },
    ambulance = {
        'ambulance',
        'ems'
    },
}
```

### Refresh Rate

Set the refresh rate for updating blips (in seconds):

```lua
Config.refreshRate = 10 -- Refresh blips every 10 seconds
```

## Installation

1. Clone the repository to your local machine.
2. Place the 

client.lua

 and 

config.lua

 files in the appropriate directory for your game server.
3. Ensure the script is loaded by your game server.

## Usage

The script will automatically track and create blips for vehicles belonging to the specified factions. No additional actions are required.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
