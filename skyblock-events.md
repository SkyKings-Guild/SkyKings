# SkyBlock Events
SkyKings has the ability to notify you when an event is coming up by sending a message in a channel of your choice.

This guide will show you how to configure it.

You will need the `manage server` permission.

# Setting an Event Channel
To get these messages, you must specify what channel you want them in. To do this, simply edit the `EVENT_CHANNEL` configuration setting.

![image](https://user-images.githubusercontent.com/49261529/123563683-ed240c80-d76a-11eb-9c5f-e35401a37e91.png)

The bot will then send messages to the channel whenever an event is:
- 30 minutes away,
- 10 minutes away,
- 5 minutes away,
- Happening now.

# Configuring the Events
The bot allows you to configure a set of settings for each individual event. The settings are as follows:
- Whether the event is enabled/disabled,
- The role to ping when the event is sent,
- The times to send the event (30 minutes, 10 minutes, 5 minutes, at the time of the event)

These settings can be modified with the `config events` command.

## Enabling/Disabling events
Disabling an event simply tells the bot to not send a message when that event occurrs. 
For example, if you don't want to recieve alerts for the Dark Auction, you can simply disable them.

To do so, you will need the event's ID. You can obtain this with the `config events` command.

To disable an event, simply run the `config events disable` command with the event's ID.

![image](https://user-images.githubusercontent.com/49261529/123564116-f615dd80-d76c-11eb-973d-b919e9a65b99.png)

To enable an event, simply run the `config events enable` command with the event's ID.

![image](https://user-images.githubusercontent.com/49261529/123564133-0332cc80-d76d-11eb-916f-38b455552776.png)

## Ping Roles
Configuring a ping role tells the bot to ping the set role whenever an alert for the specified event is sent.

To configure this, you will need the event's ID. You can obtain this with the `config events` command.

To set a ping role, run the `config events set-ping` command with the event ID and the role to ping.

You do not have to mention the role, you can use the role's name or ID.

![image](https://user-images.githubusercontent.com/49261529/123564213-560c8400-d76d-11eb-8b6c-3af7f197ed04.png)

To remove a ping role, simply don't provide the role parameter.

![image](https://user-images.githubusercontent.com/49261529/123564238-73415280-d76d-11eb-98d4-b8f7654c8086.png)

## When to Recieve Alerts
You can configure if you want an alert:
- 30 minutes before the event (30),
- 10 minutes before the event (10),
- 5 minutes before the event (5),
- At the time of the event (0).

To configure this, you will need the event's ID. You can obtain this with the `config events` command.

To add an alert time, run the `config events add-alert` command with the event's ID and the alert. (30, 10, 5, or 0)

![image](https://user-images.githubusercontent.com/49261529/123564304-cd421800-d76d-11eb-9621-ba18cf0cd664.png)

To remove an alert time, run the `config events remove-alert` command with the event's ID and the alert. (30, 10, 5, or 0)

![image](https://user-images.githubusercontent.com/49261529/123564324-dd59f780-d76d-11eb-9def-82c5c5c62d99.png)
