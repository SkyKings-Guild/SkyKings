# Commands
SkyKings has a ton of commands that you can use. Just to be helpful, here's a list of them all.

You can also view a full list of commands within Discord by typing `/` and selecting `SkyKings`.

If you're looking for how to edit the bot's config, click [here](/config.md)

Arguments can be viewed while typing out commands.

## Verification

Verification commands so you can link your Minecraft account to your Discord.

| Command | Description |
|:-------:|:---------:|
| `/verify sync` | Syncs your roles in the current server. | |
| `/unverify` | Unlinks your Minecraft account from your Discord. |
| `/verify hypixel` | Links your Minecraft account to your Discord via Hypixel. |
| `/verify website` | Links your Minecraft account to your Discord via [our Website](https://skykings.net). |
| `/verify help` | Get help with verification. |

## SkyBlock

Useful commands for Hypixel SkyBlock.

| Command | Description |
|:-------:|:-----------:|
| `/auctions` | Displays a list of a player's auctions. |
| `/bazaar` | Displays an item from the bazaar. |
| `/bits` | Displays the price of a item in the bit shop. |
| `/coins-per-bit` | Displays the items with the best coins/bit. |
| `/guildrequirements` | Displays the current guild's requirements, as well as whether or not you meet them. |
| `/lookup player` | Check if a player is a scammer or an IRL trader. |
| `/lookup user` | Check if a Discord user is a scammer or an IRL trader. |
| `/lookup list` | Lists every scammer/IRL trader in a Discord server. |
| `/lookup guild` | Lists every scammer/IRL trader in a guild. |
| `/lowestbin` | Displays the lowest BIN price for an item. |
| `/playercount` | Displays the Hypixel player count. |
| `/price` | Calculates the price of an item. |
| `/report` | Report a scammer or an IRL trader. |
| `/searchauctions` | Displays a list of auctions that matched a search query. |
| `/skyblock collection` | Displays information on a SkyBlock collection. |
| `/skyblock item` | Displays information on a SkyBlock item. |
| `/skyblock leaderboard list` | Displays a list of SkyBlock leaderboards. |
| `/skyblock leaderboard view` | Displays SkyBlock leaderboards. |
| `/skyblock skill` | Displays information on a SkyBlock skill. |
| `/skyblock time` | Displays the current Skyblock time and date. |
| `/skyblock wiki` | Searched for pages on the Hypixel Skyblock wiki. |

### All below commands are outdated and require updating with the new format.
If you would like to help update them, please feel free to open a pull request.

## Stats

Commands for displaying player statistics.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `/collections` | `<player>` | Displays a player's collections. | `cols` |
| `/dungeons` | `<player>` | Displays a player's dungeon stats. | |
| `/friends` | `<player>` | Displays a player's friends list. | |
| `/leaderboard` | `<leaderboard>` | Displays SkyBlock leaderboards. For a list of leaderboards, run the leaderboard list command. Leaderboards provided by [SkyCrypt](https://sky.shiiyu.moe). | `lb` |
| `/locate` | `<player>` | Locates a player on the Hypixel network. | |
| `/networth` | `<player>` | Displays a player's networth. Price is calculated using lowest BIN. | `nw` |
| `/player` | `<player>` | Displays a player's Hypixel profile, such as network level, socials, etc. | |
| `/profiles` | `<player>` | Displays a player's Skyblock profiles. | |
| `/skills` | `<player>` | Displays a player's skills. | |
| `/slayers` | `<player>` | Displays a player's slayers. | |
| `/weight` | `<player> [profile]` | Displays a player's weight on a specific profile. Defaults to the player's most recent profile. Powered by [hypixel-api.senither.com](https://hypixel-api.senither.com). | |

## Utility

A few useful commands that are just useful.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `k!gexp` | `<guild> <amount>` | Displays a list of users below a certain guild XP amount. | `guildxp`, `gxp` |
| `/guild` | `<guild>` | Displays a Hypixel guild. | |
| `/guildcheck` | | Displays a list of guild members that aren't in the Discord. | `gcheck` |
| `/status` | | Check the Hypixel server status. | |
| `/userinfo` | `[user]` | Displays information on a user. | `memberinfo`, `mi`, `ui` |

## Management

Commands for customizing the bot in your server!

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `/configuration view` | | Displays the server's configuration. 
| `/configuration help` | | Get help with the config! | |
| `/configuration edit` | `<key> <value>` | Edit the server's configuration. | |
| `k!config rank` | | Manage the guild's rank configuration. | |
| `k!config rank add` | `<rank> <role>` | Link a guild rank to a Discord role. | `create` |
| `k!config rank edit` | `<rank> <role>` | Edit a Discord role/guild rank link. | `modify` |
| `k!config rank remove` | `<rank>` | Delete a guild rank to Discord role link. | `delete` |
| `k!config requirements` | | Manage the guild's requirement configuration. | |
| `k!config requirements add` | `<requirement> <value>` | Creates a guild requirement. | `create` |
| `k!config requirements edit` | `<requirement> <value>` | Edits a guild requirement. | `modify` |
| `k!config requirements remove` | `<requirement>` | Deletes a guild requirement. | `delete` |
| `k!setup` | | Setup the bot! | |
| `k!tickets` | | Manages tickets. | `ticket` |
| `/ticket add` | `<member>` | Adds someone to a ticket. | |
| `/ticket close` | | Closes a ticket. | |
| `/ticket delete` | | Deletes a ticket. | |
| `/ticket help` | | Displays `help` for the ticket command. | |
| `/ticket panel` | | Manages ticket panels. | |
| `/ticket panel create` | | Creates a new ticket panel. | `make` |
| `/ticket panel delete` | `<panel>` | Deletes a ticket panel. | `remove` |
| `/ticket panel edit` | `<panel> <option> <value>` | Edits a ticket panel. | `modify` |
| `k!tickets panel help` | | Displays help for the ticket panel command. | |
| `/ticket panel info` | `<panel>` | Displays a ticket panel's config. | `show` |
| `k!tickets panel list` | | Lists every ticket panel in the server. | |
| `/ticket panel options` | | Displays a list of ticket panel options. | |
| `/ticket remove` | `<member>` | Removes someone from a ticket. | |
| `/ticket rename` | `<name>` | Renames a ticket. | |
| `/configuration unlink-guild ` | | Undoes what `setup` does. (Unlinks your Hypixel guild from the Discord server) | |

## Miscellaneous

Random commands that are somewhat useful.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `k!event` | | Main event command. | |
| `k!event end` | | Ends an event. | |
| `k!event help` | | Sends help for the `event` command. | |
| `k!event info` | | Displays information on an event. | `information` |
| `k!event join` | | Joins the currently running event. | |
| `k!event leave` | | Leave the currently running event. | |
| `k!event pos` | `[user]` | Displays a player's position in an event. | `position` |
| `k!event start` | `<event type> <channel> [ping] <duration>` | Starts an event. | `begin` |
| `k!giveaway` | | Main giveaway command. | |
| `k!giveaway help` | | Displays help for the `giveaway` command. | |
| `/giveaway start` | `<duration> <prize>` | Quickly starts a giveaway. | |
| `k!giveaway make` | | Creates a giveaway with interactive setup. | |
| `/giveaway end` | `<giveaway>` | Ends a giveaway. | |
| `/giveaway reroll` | `<giveaway>` | Rerolls a giveaway. | |

## Meta

Commands related to the bot.

| Command | Arguments | Description | Aliases |
|:-------:|:---------:|:-----------:|:-------:|
| `/apply` | | Generates a token for your bot moderator application and send you the application URL. Note: They are closed | |
| `/commands` | `[command]` | Displays command usage. | |
| `/help` | `[command]` | Displays information on a command/category. | |
| `/info` | | Displays some (kind of interesting) information about the bot. | |
| `/invite` | | Provides a URL so you can add the bot to your own server. | |
| `/ping` | | Check the bot's ping. | |
| `/request` | | Generates a request token (or regenerates it if you already have one) and sends you a form URL. | |
| `/support` | | Sends an invite to the bot's support server. | |
| `/uptime` | | Displays the bot's uptime. | |
| `/votes` | `[user]` | Displays the top voters. | |

