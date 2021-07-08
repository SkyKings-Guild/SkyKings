# Events
Events are a fairly unique feature of our bot. They work similar to the events in our [Discord](https://discord.gg/XqUQBqTh27).

## Starting an Event
Starting an event is very simple, just run the `k!event start` command with the event type, 
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
                  
