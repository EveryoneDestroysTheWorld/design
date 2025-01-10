# Matchmaking in Turf War
The player can **matchmake** with other players while they are in the lobby. They can customize the match to their liking and search for players with similar settings, or they can search based on the [round rules](./round-rules.md). 

## Matchmaking method
1. The player can join from a list of matches from the matchmaking menu, or they can create their own match with the default or preferred [round rules](./round-rules.md).
2. The game will attempt to find players in the queue with the exact round rules. If there are 8 party members, continue. After 15 seconds, the player can elect to fight bots. If they do, fill the remaining spots with bots and skip to step #4.
3. The game will sort the found players based on the closeness of the rank the player has, then choose the top 6. If there are less than 7 total participants, go back to step #2.
4. The game will wait 5 seconds; no one may leave without closing the game during this time. If anyone leaves, go back to step #2; otherwise, the game will send all participants to a private server and start the match.