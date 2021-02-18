# Configuration

SkyKings' config allows you to modify the way the bot behaves, as well as set up some useful things for your server. 
Therefore, it is very important that you understand how to use it.

The following explains how to modify the config, what it does, and why it does it.

## Keys

A config 'key' is the argument you provide in the `config edit` command, and it tells the bot what setting you want to edit.

The list of valid keys is as follows:

| Key | Description | Type |
|:---:|:-----------:|:----:|
| `PREFIX` | The bot's prefix for your server. | String (text) | 
| `VERIFICATION` | Allows you to disable verification commands. | Boolean (yes/no) |
| `SET_NICK` | Whether or not to change member's nicknames. | Boolean (yes/no) |
| `NICK_PREFIX` | Whether or not to set a prefix for a member's nickname. This requires `SET_NICK` to be on. | Boolean (yes/no) |
| `VERIFIED` | The role given to members who are verified. | Role |
| `VIP` | The role given to members with VIP. | Role |
| `VIP+` | The role given to members with VIP+. | Role |
| `MVP` | The role given to members with MVP. | Role |
| `MVP+` | The role given to members with MVP+. | Role |
| `MVP++` | The role given to members with MVP++. | Role |
| `YOUTUBE` | The role given to members with YouTube rank. | Role |
| `STAFF` | The role given to Hypixel staff members. | Role |
| `IN_GUILD` | The role given to people in the set guild. This requires the server to be linked to a Hypixel guild. | Role |
| `STORE` | The channel that purchases are sent to to be fulfulled. | Text Channel |
| `NOTIFY` | The channel that bot notifications are sent to. This currently includes scammer alerts. | Text Channel |
| `EVENTS` | The channel that global events are sent to. | Text Channel |
| `EVENTS_PING` | The role to ping when an event is started. This requires `EVENTS` to be set. | Role |
| `STATUS` | The channel to send Hypixel status updates to. | Text Channel |
| `STATUS_PING` | The role to ping for Hypixel status updates. This requires `STATUS` to be set. | Role |

There are currently 19 different configuration settings you can change.

## Editing the Config

Editing the config is quite simple. Simply run the `config edit` command with the key and value like so.

Example: `k!config edit PREFIX !`

## Linking a Guild

As you may have noticed, the `IN_GUILD` setting requires you to link your server to a guild. This can easily be done with the `setup` command, which will take you through an interactive setup process.
