# Data

The SkyKings bot uses a large amount of data to deliver the features you want. This data is stored locally in SQLite3 databases, and is usually only read by the bot.

None of the data we store will be used with malicious intent.

# Data we Store

## Economy

Used by market, shop, and order commands.

| Table | Column | Description | Used For |
|:-----:|:------:|:-----------:|:--------:|
| `SHOP` | `ITEM` | The name of the item/service for sale. | Displayed to users who request to view a server's shop. |
| `SHOP` | `ID` | The unique item ID given to every item in the shop. | Used to identify the specific item. |
| `SHOP` | `DESC` | The item/service's description. | Displayed to users who request to view the item. |
| `SHOP` | `PRICE` | The item's price. | Displayed to users who request to view the item. |
| `SHOP` | `GUILD` | The ID of the server selling the item/service. | Used to identify which server the item/service belongs to. |
| `MARKET` | `USER` | The ID of the user selling the item/service. | Used to identify which Discord user owns the item/service. | 
| `MARKET` | `UUID` | The Minecraft UUID of the user selling the item/service. | Used to identify which player owns the item/service. |
| `MARKET` | `ITEM` | The name of the item/service for sale. | Displayed to users who request to view the market. |
| `MARKET` | `ID` | The unique item ID given to every item on the market. | Used to identify the specific item |
| `MARKET` | `DESC` | The item/service's description. | Displayed to users who request to view the item. |
| `MARKET` | `PRICE` | The item's price. | Displayed to users who request to view the item. |
| `MARKET` | `SOLD` | If the item has been sold. | Used so that users can't view or buy the item once it's been sold. |
| `ORDERS` | `USER` | The ID of the user who created the order. | Used to identify which Discord user purchased the item/service. |
| `ORDERS` | `UUID` | The Minecraft UUID of the user ordering the item/service. | Used to identify which player purchased the item/service. |
| `ORDERS` | `ID` | The unique item ID given to every order created. | Used to identify the specific order. |
| `ORDERS` | `SELLER` | The ID of the user selling the item/service. | Used to identify which Discord user owns the item/service. |
| `ORDERS` | `TYPE` | The type of order this is. Can be either `GLOBAL_MARKET` or `GUILD_SHOP`. | Used to figure out what table to request the item from. |
| `ORDERS` | `ITEM` | The ID of the item being sold. | Used to retrieve the item's data. |
| `ORDERS` | `COMPLETE` | Whether or not the order has been complete. | Used to figure out whether or not you can complete/cancel the order. |

## Event

Used for managing events within the bot.

This database only exists while an event is running, and is immediatly deleted once it ends.

| Table | Column | Description | Used For |
|:-----:|:------:|:-----------:|:--------:|
| `USERS` | `MEMBER` | The member's ID. | Used to DM the top 10 after the event ends. |
| `USERS` | `UUID` | The player's UUID. | Used to request player data from the Hypixel API. |
| `USERS` | `STARTING` | The amount of `x` the player had when they joined the event. | Used to calculate the amount of `x` the player has gained since they joined the event. |
| `USERS` | `POS` | The player's position in the event. | Used by the `event pos` command to show a player's position. |
| `USERS` | `IGNORE` | The profiles that should be ignored until their API settings are enabled. | Used to prevent people from disabling their API, joining, then enabling it again to get all their `x` to count. |
| `USERS` | `EVENTXP` | The amount of `x` that the player has in the event. | Used by the `event pos` command to show the player's progress. |
| `MESSAGES` | `GUILD` | The ID of the server the message belongs to. | Used for updating the event message. |
| `MESSAGES` | `CHANNEL` | The ID of the channel the message belongs to. | Used for updating the event message. |
| `MESSAGES` | `MESSAGE` | The ID of the message to be updated. | Used for updating the event message. |

## Giveaway

Used for managing giveaways.

Giveaways are deleted a week after their scheduled end date.

| Table | Column | Description | Used For |
|:-----:|:------:|:-----------:|:--------:|
| `GIVEAWAYS` | `CHANNEL` | The ID of the channel that the message belongs to. | Used for retrieving the giveaway message. |
| `GIVEAWAYS` | `MESSAGE` | The ID of the giveaway message. | Used for retrieving giveaway entries and updating the message once the giveaway ends. |
| `GIVEAWAYS` | `PRIZE` | The giveaway's prize. | Used for editing the giveaway message once it ends, and providing the prize in the ending message. |
| `GIVEAWAYS` | `ENDS` | The time that the giveaway ends. | Used for automatically ending the giveaway. |
| `GIVEAWAYS` | `ENDCONTENT` | The message to be shown when the giveaway ends. | Used for showing the message when the giveaway ends. |
| `GIVEAWAYS` | `CREATED` | The ID of the user who created the giveaway. |  Used for editing the giveaway message once it ends. |
| `GIVEAWAYS` | `HOSTED` | The ID of the user that's sponsoring the giveaway. | Used for editing the giveaway message once it ends. |
| `GIVEAWAYS` | `REQUIREMENTS` | The giveaway's requirements. | Not used at all, as it's not implemented yet. |
| `GIVEAWAYS` | `CONTENT` | The message sent when the giveaway started. | Used for editing the giveaway message once it ends. |
| `GIVEAWAYS` | `WINNERS` | The amount of winners the giveaway should have. | Used for choosing a number of winners. |
| `GIVEAWAYS` | `ENDED` | Whether or not the giveaway is ended. | Used to decide whether or not it can be rerolled or ended. |
| `GIVEAWAYS` | `GUILD` | The server the giveaway is in. | Used to decide whether or not you can end the giveaway, as the message converter works for messages in all servers. |

## Guilds

Mostly guild configuration.

| Table | Column | Description | Used For |
|:-----:|:------:|:-----------:|:--------:|
| `GUILDS` | `DISCORD` |  The ID of the server that the configuration belongs to. | Used for bot configuration. |
| `GUILDS` | `GUILD` | The ID of the Hypixel guild that the server is linked to. | Used for bot configuration. |
| `GUILDS` | `PREFIX` | The server's bot prefix. | Used for bot configuration. |
| `GUILDS` | `VERIFIED` | The server's verified role. | Used for bot configuration. |
| `GUILDS` | `VIP` | The server's VIP role. | Used for bot configuration. |
| `GUILDS` | `VIP_P` | The server's VIP+ role. | Used for bot configuration. |
| `GUILDS` | `MVP` | The server's MVP role. | Used for bot configuration. |
| `GUILDS` | `MVP_P` | The server's MVP+ role. | Used for bot configuration. |
| `GUILDS` | `MVP_PP` | The server's MVP++ role. | Used for bot configuration. |
| `GUILDS` | `YT` | The server's YouTube Rank role. | Used for bot configuration. |
| `GUILDS` | `STAFF` | The server's Hypixel Staff role. | Used for bot configuration. |
| `GUILDS` | `STORE_CHANNEL` | The server's store channel. | Used for bot configuration. |
| `GUILDS` | `IN_GUILD` | The server's role for guild members. | Used for bot configuration. |
| `GUILDS` | `SETNICK` | Whether or not to change member's nicknames. | Used for bot configuration. |
| `GUILDS` | `NICKPREFIX` | Whether or not to add a rank prefix to member's nicknames. | Used for bot configuration. |
| `GUILDS` | `NOTIFICATIONS` | The server's scammer notification channel. | Used for bot configuration. |
| `GUILDS` | `VERIFY` | Whether or not verification is enabled. | Used for bot configuration. |
| `GUILDS` | `EVENTS` | The server's event channel. | Used for bot configuration. |
| `GUILDS` | `EVENTS_ROLE` | The server's event ping role. | Used for bot configuration. |
| `GUILDS` | `HYPIXEL_STATUS` | The server's Hypixel status channel. | Used for bot configuration. |
| `GUILDS` | `STATUS_ROLE` | The server's Hypixel status ping role. | Used for bot configuration. |
| `GUILDS` | `GIVEAWAYS` | The server's giveaway role. | Used for bot configuration. |
| `RANKS` | `GUILD` | The ID of the server the rank belongs to. | Used for guild rank syncing. |
| `RANKS` | `ROLE` | The ID of the role the rank belongs to. | Used for guild rank syncing. |
| `RANKS` | `RANK` | The name of the rank. | Used for guild rank syncing. |

## Scammers

The bot's scammer list.


| Table | Column | Description | Used For |
|:-----:|:------:|:-----------:|:--------:|
| `PLAYERS` | `UUID` | The player's UUID. | Looking up scammers/IRL traders. |
| `PLAYERS` | `REASON` | The reason the player is flagged as such | Looking up scammers/IRL traders. |
| `PLAYERS` | `TYPE` | If the player is a scammer or an IRL trader | Looking up scammers/IRL traders. |
| `PLAYERS` | `MOD` | The bot mod that added the scammer. | Nothing, yet. |
| `PLAYERS` | `REMOVED` | Whether or not the entry was removed. | Used for deciding whether or not to show the entry. |
| `PLAYERS` | `REMOVER` | The bot mod that removed the entry. | Nothing, yet. |
| `PLAYERS` | `REMOVE_REASON` | The reason the entry was removed. | Nothing, yet. |
| `PLAYERS` | `ID` | The entry ID. | Used for removing entries. |
| `USERS` | `USER` | The user's ID. | Looking up scammers/IRL traders. |
| `USERS` | `REASON` | The reason the player is flagged as such | Looking up scammers/IRL traders. |
| `USERS` | `TYPE` | If the player is a scammer or an IRL trader | Looking up scammers/IRL traders. |
| `USERS` | `MOD` | The bot mod that added the scammer. | Nothing, yet. |
| `USERS` | `REMOVED` | Whether or not the entry was removed. | Used for deciding whether or not to show the entry. |
| `USERS` | `REMOVER` | The bot mod that removed the entry. | Nothing, yet. |
| `USERS` | `REMOVE_REASON` | The reason the entry was removed. | Nothing, yet. |
| `USERS` | `ID` | The entry ID. | Used for removing entries. |

## Verification

Mainly for linking users to players.

| `USERS` | `USER` | The ID of the user. | Checking if a user is linked, who a player is linked to, etc. |
| `USERS` | `UUID` | The UUID of the player. | Checking if a player is linked, who a user is linked to, etc. |
