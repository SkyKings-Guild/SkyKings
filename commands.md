# Commands
SkyKings has a ton of commands that you can use. Here's a list of them all.

If you're looking for how to edit the bot's config, click [here](/config.md)

Note: Do not literally type `<>` and `[]`

Note: Aliases for subcommands will not contain the parent command.

## How to Read
Optional: `[foo]` means that this argument can be ignored.

Required: `<foo>` means that you must use this argument for the command to work
  
Many: `<foos...>` or `[foos...]` means that you can specify more than one. 
  
Multi-word Arguments: If you wish you use an argument with more than one word, use "double quotes" to let the bot you know what you want. 
Most of the time, if a multi-word argument is at the end of a command, this is not necessary.

## Verification

Verification commands so you can link your Minecraft account to your Discord.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `verify` | `<player>` | Links your Minecraft account to your Discord via Hypixel. | `link` |
| `unverify` | | Unlinks your Minecraft account from your Discord. | `unlink` |
| `sync` | | Syncs your roles in the current server. | |
| `verifyhelp` |  | Get help with verification. | `linkhelp` |

## Economy

Commands for buying and selling of items and/or services in Hypixel Skyblock.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `shop` |  | View the server shop. | `store` | | `add reactions` |
| `shop create` | `<item> <price> <description>` | Add an item to the server shop. | `add` |
| `shop delete` | `<product id>` | Remove an item from the server shop. | `delete` |
| `shop edit` | `<product id> <option> <value>` | Edit an item on the guild shop. Valid options are `price`, `desc`, and `name`. | `change` |
| `shop info` | `<product id>` | Displays an item on the server's shop. | `information` |
| `shop buy` | `<product id>` | Requests to purchase an item on the server's shop. | `purchase`, `order` |
| `shop help` | | Displays help for the `shop` command. | |
| `order` | | Main command for managing orders. | |
| `order help` | | Displays help for the `order` command. | |
| `order cancel` | `<order id>` | Cancels an order. This can only be used by the seller. | |
| `order complete` | `<order id>` | Completes an order. This can only be used by the seller. | |
| `market` | | View the global market. | |
| `market add` | `<item> <price> <description>` | Add an item to the global market. | `create` |
| `market delete` | `<product id>` | Remove an item from the global market. | `remove` |
| `market edit` | `<product id> <option> <value>` | Edit an item on the global market. Valid options are `price`, `desc`, and `name`. | `change` |
| `market info` | `<product id>` | Displays an item on the global market. | `information` |
| `market buy` | `<product id>` | Requests to purchase an item off the global market. | `purchase`, `order` |
| `market help` | | Displays help for the `market` command. | |

## SkyBlock

Useful commands for Hypixel SkyBlock.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `report` | `[player]` | Report a scammer or an IRL trader. | |
| `lookup` | `<player>` | Check if a user is a scammer or an IRL trader. | `scammer`, `trader` |
| `scammers` | | Lists every scammer/IRL trader in a Discord server. | |
| `auctions` | `<player>` | Displays a list of a player's auctions. | `ah`, `auctionhouse` |
| `bazaar` | `<item>` | Displays an item from the bazaar. | `baz` |
| `playercount` | | Displays the SkyBlock player count. | `pc` |
| `slayers` | `<player>` | Displays a player's slayers. | |
| `skills` | `<player>` | Displays a player's skills. | |
| `searchauctions` | `<query>` | Displays a list of auctions that matched a search query. | `searchah` |
| `lowestbin` | `<item>` | Displays the lowest BIN price for an item. | `lbin` |
| `price` | `<item>` | Displays the price of an item. Uses `Jerry the Price Checker`'s database. | |

## Utility

A few useful commands that are just useful.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `gexp` | `<guild> <amount>` | Displays a list of users below a certain guild XP amount. | `guildxp`, `gxp` |
| `status` | | Check the Hypixel server status. | |
| `userinfo` | `<user>` | Displays information on a user. | `memberinfo`, `mi`, `ui` |

## Management

Commands for customizing the bot in your server!

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `config` | | Displays the server's configuration. | `configuration` |
| `config help` | | Get help with the config! | |
| `config edit` | `<key> <value>` | Edit the server's configuration. | |
| `rank` | | Manage the guild's rank configuration. | |
| `rank add` | `<rank> <role>` | Link a guild rank to a Discord role. | `create` |
| `rank edit` | `<rank> <role>` | Edit a Discord role/guild rank link. | `modify` |
| `rank remove` | `<rank>` | Delete a guild rank to Discord role link. | `delete` |
| `setup` | | Setup the bot! | |
| `unlink_guild` | | Undoes what `setup` does. (Unlinks your Hypixel guild from the Discord server) | |

## Miscellaneous

Random commands that are somewhat useful.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `event` | | Main event command. | |
| `event join` | | Joins the currently running event. | |
| `event leave` | | Leave the currently running event. | |
| `event pos` | `[user]` | Displays a player's position in an event. | `position` |
| `event info` | | Displays information on an event. | `information` |
| `event start` | `<event type>` | Starts an event. | `begin` |
| `event end` | | Ends an event. | |

## Meta

Commands related to the bot.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `uptime` | | Displays the bot's uptime. | |
| `invite` | | Provides a URL so you can add the bot to your own server. | |
| `support` | | Sends an invite to the bot's support server. | |
| `info` | | Displays some (kind of interesting) information about the bot. | |
| `ping` | | ~~play ping-pong~~ Check the bot's ping. | |
| `help` | `[command]` | Displays information on a command/category. | |

## Restricted

Restricted commands shall remain undocumented, as there really isn't any reason to document them.

