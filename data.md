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

