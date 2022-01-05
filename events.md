# Events
Events are a fairly unique feature of our bot. They work similar to the events in our [Discord](https://discord.gg/XqUQBqTh27).

## Starting an Event
Starting an event is very simple, just run the `/event start` command with the event type, 
the channel the leaderboard should be in, a role to ping (optional), and the event duration.

![image](https://user-images.githubusercontent.com/49261529/124861527-a0a9af80-df68-11eb-9d7b-6dd08313df95.png)

The bot will then send a leaderboard which will update every 6 hours, or every hour if you have premium.

![image](https://user-images.githubusercontent.com/49261529/124861578-b61ed980-df68-11eb-8dc4-7e92f1e68b13.png)

## Event Types
When starting an event, it's quite important to know what type of event you're starting, and what it tracks.

Below is a list of event types and the XP they track.

| Event Type | Description |
|:----------:|:-----------:|
| `SKILL` | Tracks Farming, Mining, Combat, Foraging, Fishing, Enchanting, Alchemy, Carpentry, Runecrafting and Taming. |
| `SKILL_*` | Same as above, but tracks a specific skill (for example, `SKILL_FARMING` would track farming XP).
| `SLAYERS` | Tracks slayer XP. |
| `CATACOMBS` | Tracks catacombs XP. |
| `WEIGHT` | Tracks weight. Calculations are provided by Senither. |
| `WEIGHTED_XP` | Tracks 3% of the Alchemy skill, 12% of Farming, 60% of Mining, 80% Combat, 115% Foraging, 250% Fishing, 10% Enchanting, 50% Catacombs XP and 100% slayer XP. 100% is normal XP gain. |

If your server has premium, you can prefix the event type with `GVG_` (for example, `GVG_WEIGHTED_XP`) and it will make the event a Guilds vs Guilds event.

## Joining an Event
There are 2 ways to join an event:
1. Clicking the 'Join Event' button on the leaderboard,
2. Running the `/event join` command.

![image](https://user-images.githubusercontent.com/49261529/124862554-7bb63c00-df6a-11eb-8245-a180fa79e43f.png)

![image](https://user-images.githubusercontent.com/49261529/124862596-8a045800-df6a-11eb-949c-29f354df09d9.png)

## Leaving an Event
If for whatever reason you would like to leave an event, you can run the `event leave` command and select `Yes`.

![image](https://user-images.githubusercontent.com/49261529/124862658-a6a09000-df6a-11eb-84b0-e3b5187a9ad3.png)

![image](https://user-images.githubusercontent.com/49261529/124862674-ab654400-df6a-11eb-9ea4-913dc175e6fc.png)

## Checking your Position
There are 2 ways to check your position in an event:
1. Clicking the 'Check Position' button on the leaderboard,
2. Running the `/event position` command.

![image](https://user-images.githubusercontent.com/49261529/124862783-d94a8880-df6a-11eb-9512-bc737836b833.png)

![image](https://user-images.githubusercontent.com/49261529/124862799-df406980-df6a-11eb-926a-e1838defe7ac.png)




                  
