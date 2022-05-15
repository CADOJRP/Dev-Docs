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
____
##### Get Player Bank ID
**Arguments:** Player ID (or source)

**Returns:** Player BankID (or null if not found)
```Lua
exports['CADOJRPv2'].getPlayerBankID(playerid)
```
____
##### Get Player Wallet/Cash Balance
**Arguments:** Player ID (or source)

**Returns:** Wallet/Cash Balance as Int
```Lua
exports['CADOJRPv2'].getWalletBalance(playerid)
```

____
##### Get Player Bank Balance
**Arguments:** Player ID (or source)

**Returns:** Bank Balance as Int
```Lua
exports['CADOJRPv2'].getBankBalance(playerid)
```

____
##### Get BankID Wallet/Cash Balance
**Arguments:** Bank ID (Use getPlayerBankID() or arbirtary value)

**Returns:** Wallet/Cash Balance as Int
```Lua
exports['CADOJRPv2'].getWalletBalanceFromBankID(bankid)
```

____
##### Get BankID Bank Balance
**Arguments:** Bank ID (Use getPlayerBankID() or arbirtary value)

**Returns:** Bank Balance as Int
```Lua
exports['CADOJRPv2'].getBankBalanceFromBankID(bankid)
```

____
##### Add Bank Money to BankID
**Arguments:** Bank ID, Value

**Returns:** True/False
```Lua
exports['CADOJRPv2'].addBankMoney(bankid, 100)
```
____
##### Add Cash/Wallet Money to BankID
**Arguments:** Bank ID, Value

**Returns:** True/False
```Lua
exports['CADOJRPv2'].addWalletMoney(bankid, 100)
```

____
##### Remove Bank Money from BankID
**Warning:** This does not automatically check if they can afford it. This can cause someone to go negative balance.
**Arguments:** Bank ID, Value

**Returns:** True/False
```Lua
exports['CADOJRPv2'].removeBankMoney(bankid, 100)
```
____
##### Remove Cash/Wallet Money from BankID
**Warning:** This does not automatically check if they can afford it. This can cause someone to go negative balance.

**Arguments:** Bank ID, Value

**Returns:** True/False
```Lua
exports['CADOJRPv2'].removeWalletMoney(bankid, 100)
```
