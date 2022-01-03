# Configuration

SkyKings' config allows you to modify the way the bot behaves, as well as set up some useful things for your server. 
Therefore, it is very important that you understand how to use it.

The following explains how to modify the config, what it does, and why it does it.

# Bot Configuration

## Keys

A config 'key' is the argument you provide in the `config edit` command, and it tells the bot what setting you want to edit.

The list of valid keys is as follows:

### General Bot Configuration
| Key | Description | Type | Example |
|:---:|:-----------:|:----:|:-------:|
| `PREFIX` | The bot's prefix for your server. This will be removed in April of 2022. | String (text) | `k!` | 
| `TRIGGERS` | Whether or not the bot should reply to normal messages. This may be removed April due to the message content restriction. Learn more [here](https://support-dev.discord.com/hc/en-us/articles/4404772028055-Message-Content-Privileged-Intent-for-Verified-Bots). | Boolean (yes/no) | `on` |
| `STORE` | The channel that purchases are sent to to be fulfulled. | Text Channel | `#store-alerts` |
| `NOTIFY` | The channel that bot notifications are sent to. This currently includes scammer alerts. | Text Channel | `#scammer-notifications` |
| `STATUS` | The channel to send Hypixel status updates to. | Text Channel | `#hypixel-status` |
| `STATUS_PING` | The role to ping for Hypixel status updates. This requires `STATUS` to be set. | Role | `@Status Ping` |
| `GIVEAWAYS` | The role that should be able to run giveaways. | Role | `@Giveaway Runner` |
| `SCAMMER_ACTION` | The action that should be taken when scammers join your server. | `kick`, `ban`, Role | `kick`, `ban`, `@Scammer` |
| `TRADER_ACTION` | The action that should be taken when IRL traders join your server. | `kick`, `ban`, Role | `kick`, `ban`, `@IRL Trader` |
| `NEWS` | The channel for Hypixel news to be sent to. | Text Channel | `#news` |
| `NEWS_PING` | The role to ping for Hypixel news. | Role | `@News Ping` |
| `PATCHNOTES` | The channel for SkyBlock patchnotes to be sent to. | Text Channel | `#patchnotes` |
| `PATCHNOTES_PING` | The role to ping for SkyBlock patchnotes. | Role | `@Patchnotes Ping` |
| `MEMBER_COUNT` | The channel that should be edited to display guild members. (Premium Only) | Voice Channel | `#Member Count` |
| `SKYBLOCK_DATE` | The channel that should be edited to display the current SkyBlock date. | Voice Channel | `#Skyblock Date` 
| `EVENT_CHANNEL` | The channel that SkyBlock events should be sent to. Learn more [here](https://github.com/SkyKings-Guild/SkyKings/blob/main/skyblock-events.md). | Text Channel | `#skyblock-events` |
| `GLOBAL_EVENT_CHANNEL` | The channel that global events should be sent to. (Premium Only) | Text Channel | `#events` |
| `FETCHUR` | The channel that Fetchur items should be sent to. | Text Channel | `#fetchur` |
| `FETCHUR_PING` | The role to ping for Fetchur items. | Role | `@Daily Fetchur` |



### Verification Configuration
| Key | Description | Type | Example |
|:---:|:-----------:|:----:|:-------:|
| `VERIFICATION` | Allows you to disable verification commands. | Boolean (yes/no) | `on` |
| `NICK` | The format a member's nickname should be in. | String (text) - Supports variables `name`, `network_level`, `rank` and `cata_level`. | `[{rank}] {name}` |
| `VERIFIED` | The role given to members who are verified. | Role | `@Verified` |
| `VIP` | The role given to members with VIP. | Role | `@VIP` |
| `VIP+` | The role given to members with VIP+. | Role | `@VIP+` |
| `MVP` | The role given to members with MVP. | Role | `@MVP` |
| `MVP+` | The role given to members with MVP+. | Role | `@MVP+` |
| `MVP++` | The role given to members with MVP++. | Role | `@MVP++` |
| `YOUTUBE` | The role given to members with YouTube rank. | Role | `@YT` |
| `STAFF` | The role given to Hypixel staff members. | Role | `@Hypixel Staff` |
| `IN_GUILD` | The role given to people in the set guild. This requires the server to be linked to a Hypixel guild. | Role | `@Guild Member` |


There are currently 31 different configuration settings you can change.

## Editing the Config

Editing the config is quite simple. Simply run the `config edit` command with the key and value like so.

Example: `k!config edit PREFIX !`

If you want to remove a config setting, just do `k!config edit <setting> reset`.

## Linking a Guild

As you may have noticed, the `IN_GUILD` setting requires you to link your server to a guild. This can easily be done with the `setup` command, which will take you through an interactive setup process. Ranks and guild requirements also require this.

# Guild Ranks

To add a guild rank to the bot, simply run the `config ranks add` command with the `rank` name and the `role`.

Example: `k!config ranks add Member @Role`

You can then edit it with `config ranks edit` and remove it with `config ranks remove`.

# Guild Requirements

To add a guild requirement to the bot, simply run the `config requirements add` command with the `requirement` and the `value`.

Example: `k!config requirements add weight 5000`

You can then edit it with `config requirements edit` and remove it with `config requirements remove`.

To view a full list of requirements, run the `config requirements help` command.
