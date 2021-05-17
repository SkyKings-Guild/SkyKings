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
| `sync` | | Syncs your roles in the current server. | |
| `unverify` | | Unlinks your Minecraft account from your Discord. | `unlink` |
| `verify` | `<player>` | Links your Minecraft account to your Discord via Hypixel. | `link` |
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
| `auctions` | `<player>` | Displays a list of a player's auctions. | `ah`, `auctionhouse` |
| `bazaar` | `<item>` | Displays an item from the bazaar. | `baz` |
| `bits` | `<item>` | Displays the price of a item in the bit shop. | `bit` |
| `coinsperbit` | | Displays the item with the best coins/bit. | `coinperbit`, `cpb` |
| `collection` | `<collection>` | Displays information on a SkyBlock collection. | 
| `guildrequirements` | `<player>` | Displays the current guild's requirements, as well as whether or not you meet them. | `guildrequirement`, `greq`, `greqs` |
| `lookup` | `<player>` | Check if a user is a scammer or an IRL trader. | `scammer`, `trader` |
| `lowestbin` | `<item>` | Displays the lowest BIN price for an item. | `lbin` |
| `playercount` | | Displays the SkyBlock player count. | `pc` |
| `price` | `<item>` | Displays the price of an item. Uses `Jerry the Price Checker`'s database. | |
| `report` | `[player]` | Report a scammer or an IRL trader. | |
| `scammers` | | Lists every scammer/IRL trader in a Discord server. | |
| `searchauctions` | `<query>` | Displays a list of auctions that matched a search query. | `searchah` |
| `skill` | `<skill>` | Displays information on a SkyBlock skill. | |

## Stats

Commands for displaying player statistics.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `collections` | `<player>` | Displays a player's collections. | `cols` |
| `dungeons` | `<player>` | Displays a player's dungeon stats. | |
| `friends` | `<player>` | Displays a player's friends list. | |
| `leaderboard` | `<leaderboard>` | Displays SkyBlock leaderboards. For a list of leaderboards, run the leaderboard list command. Leaderboards provided by [SkyCrypt](https://sky.shiiyu.moe). | `lb` |
| `locate` | `<player>` | Locates a player on the Hypixel network. | |
| `networth` | `<player>` | Displays a player's networth. Price is calculated using lowest BIN. | `nw` |
| `player` | `<player>` | Displays a player's Hypixel profile, such as network level, socials, etc. | |
| `profiles` | `<player>` | Displays a player's Skyblock profiles. | |
| `skills` | `<player>` | Displays a player's skills. | |
| `slayers` | `<player>` | Displays a player's slayers. | |
| `weight` | `<player> [profile]` | Displays a player's weight on a specific profile. Defaults to the player's most recent profile. Powered by [hypixel-api.senither.com](https://hypixel-api.senither.com). | |

## Utility

A few useful commands that are just useful.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `gexp` | `<guild> <amount>` | Displays a list of users below a certain guild XP amount. | `guildxp`, `gxp` |
| `guild` | `<guild>` | Displays a Hypixel guild. | |
| `guildcheck` | | Displays a list of guild members that aren't in the Discord. | `gcheck` |
| `status` | | Check the Hypixel server status. | |
| `userinfo` | `[user]` | Displays information on a user. | `memberinfo`, `mi`, `ui` |

## Management

Commands for customizing the bot in your server!

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `config` | | Displays the server's configuration. | `configuration` |
| `config help` | | Get help with the config! | |
| `config edit` | `<key> <value>` | Edit the server's configuration. | |
| `config rank` | | Manage the guild's rank configuration. | |
| `config rank add` | `<rank> <role>` | Link a guild rank to a Discord role. | `create` |
| `config rank edit` | `<rank> <role>` | Edit a Discord role/guild rank link. | `modify` |
| `config rank remove` | `<rank>` | Delete a guild rank to Discord role link. | `delete` |
| `config requirements` | | Manage the guild's requirement configuration. | |
| `config requirements add` | `<requirement> <value>` | Creates a guild requirement. | `create` |
| `config requirements edit` | `<requirement> <value>` | Edits a guild requirement. | `modify` |
| `config requirements remove` | `<requirement>` | Deletes a guild requirement. | `delete` |
| `setup` | | Setup the bot! | |
| `tickets` | | Manages tickets. | `ticket` |
| `tickets add` | `<member>` | Adds someone to a ticket. | |
| `tickets close` | | Closes a ticket. | |
| `tickets delete` | | Deletes a ticket. | |
| `tickets help` | | Displays `help` for the ticket command. | |
| `tickets panel` | | Manages ticket panels. | |
| `tickets panel create` | | Creates a new ticket panel. | `make` |
| `tickets panel delete` | `<panel>` | Deletes a ticket panel. | `remove` |
| `tickets panel edit` | `<panel> <option> <value>` | Edits a ticket panel. | `modify` |
| `tickets panel help` | | Displays help for the ticket panel command. | |
| `tickets panel info` | `<panel>` | Displays a ticket panel's config. | `show` |
| `tickets panel list` | | Lists every ticket panel in the server. | |
| `tickets panel options` | | Displays a list of ticket panel options. | |
| `tickets remove` | `<member>` | Removes someone from a ticket. | |
| `tickets rename` | `<name>` | Renames a ticket. | |
| `unlink_guild` | | Undoes what `setup` does. (Unlinks your Hypixel guild from the Discord server) | |

## Miscellaneous

Random commands that are somewhat useful.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `event` | | Main event command. | |
| `event end` | | Ends an event. | |
| `event help` | | Sends help for the `event` command. | |
| `event info` | | Displays information on an event. | `information` |
| `event join` | | Joins the currently running event. | |
| `event leave` | | Leave the currently running event. | |
| `event pos` | `[user]` | Displays a player's position in an event. | `position` |
| `event start` | `<event type> <channel> [ping] <duration>` | Starts an event. | `begin` |
| `giveaway` | | Main giveaway command. | |
| `giveaway help` | | Displays help for the `giveaway` command. | |
| `giveaway start` | `<duration> <prize>` | Quickly starts a giveaway. | |
| `giveaway make` | | Creates a giveaway with interactive setup. | |
| `giveaway end` | `<giveaway>` | Ends a giveaway. | |
| `giveaway reroll` | `<giveaway>` | Rerolls a giveaway. | |

## Meta

Commands related to the bot.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `apply` | | Generates a token for your bot moderator application and send you the application URL. | |
| `commands` | `[command]` | Displays command usage. | |
| `help` | `[command]` | Displays information on a command/category. | |
| `info` | | Displays some (kind of interesting) information about the bot. | |
| `invite` | | Provides a URL so you can add the bot to your own server. | |
| `ping` | | ~~play ping-pong~~ Check the bot's ping. | |
| `support` | | Sends an invite to the bot's support server. | |
| `uptime` | | Displays the bot's uptime. | |
| `votes` | `[user]` | Displays the top voters. | |

## Restricted

Restricted commands shall remain undocumented, as there really isn't any reason to document them.

