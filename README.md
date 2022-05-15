# CADOJRP Server Exports

____
##### Check if Player is online.
**Arguments:** Player ID (or source)
**Returns:** True/False
```Lua
exports['CADOJRPv2'].playerOnline(playerId)
```
____
##### Check if Source is server console.
**Arguments:** Source
**Returns:** True/False
```Lua
exports['CADOJRPv2'].isConsole(source)
```
____
##### Hex To Decimal
**Arguments:** Hexadecimal Value
**Returns:** Decimal Value as String
```Lua
exports['CADOJRPv2'].hexToDec(hexValue)
```
____
##### Get Unix Time
**Returns:** Unix Timestamp (Seconds since 1970)
```Lua
exports['CADOJRPv2'].unixTime()
```
____
##### Chat Message
**Arguments:** Message, To, IsSystem ([CADOJRP] Prefix)
**Returns:** True/False
```Lua
exports['CADOJRPv2'].chatMessage('Hello!', -1, false) -- Will display Hello! to all players
exports['CADOJRPv2'].chatMessage('Hello!', -1, true) -- Will display [CADOJRP] Hello! to all players
```
____
##### Console Message
**Arguments:** Message, Type (error, warning, info, debug (will default to info))
**Returns:** Nothing
```Lua
exports['CADOJRPv2'].consoleMessage('Exploit Detected!', 'error') -- Will display [CADOJRP] [ERROR] Exploit Detected! in the server console.
```
____
##### Get Player UUID
**Arguments:** Player ID (or source)
**Returns:** Player UUID (or null if not found)
```Lua
exports['CADOJRPv2'].getPlayerUUID(playerid)
```
