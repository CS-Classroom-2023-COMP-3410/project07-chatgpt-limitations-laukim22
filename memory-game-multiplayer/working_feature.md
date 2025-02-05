I asked chatGPT this question:

"Here's code. Make this multiplayer--display which player's turn it is, and keep track of the number of pairs/matches each player gets. If they get it right, they get another turn."
I also fed it both the index.html and js file

After two failed generations (just literally said failed generation), it worked.

When asked to explain what changes were made, chatGPT gave me this:
"Added Player Tracking:

Introduced an array players = ["Player 1", "Player 2"] to store player names.
Added a currentPlayer variable to keep track of whose turn it is.
Score Tracking:

Created an array scores = [0, 0] to store each player's score.
When a player finds a match, their score increases.
Turn Management:

If a player gets a match, they keep their turn.
If they don’t, the turn switches to the other player with the switchPlayer() function.
UI Updates for Players:

Created playerTurnDisplay and playerScoresDisplay elements to show whose turn it is and the scores.
Updated the UI each turn using updatePlayerDisplay().
Game Reset Adjustments:

When restarting, resets scores and ensures Player 1 starts first."