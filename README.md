# SkriptMultiEval
This script allow you to use multiple codes to evaluate in-game using `/#` command

## Why?
Skript has a built-in evaluate effect but it only evaluates one line code at a time, this script allows you to do multiple `single line` effects at a time.

What is `multiple single line effect`? this script can't do loops or indentations, but it can do this `/# set {_i} ti "Test" -> broadcast {_i}`

## Docs
```
#! Use $me to get the player parsed as a player type (not surrounded by quotation marks "") - ex. (give 1 stone to $me) this will be parsed as (give 1 stone to "SkriptDev" parsed as player)
#! Use $player to get the player parsed as a player type (when surrounded by quotation marks "") - ex. (send "%tool of $player%") this will be parsed as (send "%tool of ""SkriptDev"" parsed as offlineplayer%")

#! Use $name to get the player name parsed as text
#! Use $uuid to get the uuid of player

#! Use $PlayerName$ to get some player parsed as a offlineplayer type (not surrounded by quotation marks "") - ex. (give 1 stone to $SkriptDev$) this will be parsed as (give 1 stone to "SkriptDev" parsed as player)
#! Use $$PlayerName$ to get some player parsed as a offlineplayer type (surrounded by quotation marks "") - ex. (send "%tool of $$SkriptDev$%") this will be parsed as (send "%tool of ""SkriptDev"" parsed as offlineplayer%")

#! Use " -> " without the quotes to use multi lines (Note the spaces around the -> are important) - ex. (set {_i} to "Test" -> broadcast {_i})

#! Command to use this '/#' without quotes to use the function
#! Permission required: 'skript.multieval'
```

## Requirements
[Skript](https://github.com/SkriptLang/Skript/)

[TuSKe](https://skripttools.net/dl/TuSKe+1.8.3-PikachuPatch-v3.jar)


## Examples
`/# set $me's tool to diamond sword of sharpness 1` - Set sender's tool to diamond sword of sharpness 1

`/# send "%name of $player's tool%"` - Name of sender's tool

`/# send "%$$SkriptDev$'s tool%"` - Send tool of a player named "SkriptDev"

`/# set $me's tool to stone -> broadcast "%$player's tool%"` - Set sender's tool to stone then broadcast it
