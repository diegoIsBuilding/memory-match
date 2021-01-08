# Memory Match
## Functionality Overview

1. Create a matching game in which a player attempts to match the card images.
2. There are a total of 18 cards.
3. Tracked the total number of games played, total number of matches for the current game, and health score.
4. The cards are displayed face down and "flip" over when they are clicked.
5. Two cards can be flipped each round.
6. If the flipped cards match - keep the matched card on display and increment a point to matches.
7. If the flipped cards do Not match - flip the cards back over - and update the health score.
8. Once 9 matches occurs - a modal is displayed to tell the user they have won - display a button that will allow for a game reset
9. Resetting the game performs the following actions:
    - All cards are flipped back over
    - The number of games played is increased
    - The total number of matches are reset
    - The accuracy percentage is reset to 0%
    
# Feature Sets
1. User can view the memory match game 
    - Design a simple grid system for use in constructing the layout.
    - Identify what primary elements you will need to divide the page correctly.
    - Identify the child elements you will need in each of the primary elements.
    - Build the initial HTML skeleton based on the required element list.
    - Implement the correct CSS to style the skeleton based on the Design Doc
2. User can flip board game cards
    - Adding additional HTML to create the front and back cards.
    - Adding additional CSS to for the new front and back background images, and necessary positioning changes.
    - Adding click functionality to the cards.
    - Creating a CSS class which will be used to hide the back of the cards when they are clicked.
    - Click functionality which will use the CSS from the previous step to hide the back of the card and reveal the front of the card that is clicked.
3. User can match two cards 
    - Create global variables to store references to cards which are clicked.
    - Create the logic to properly store the card references for the two cards clicked each round.
    - Retrieve the classes on the sibling elements of the cards which were clicked and stored.
    - Compare the classes of the sibling elements to see if they match.
    - Flipping the cards back if the classes for the background images do not match.
    - Creating a delay before the cards which don't match are flipped back.
    - Preventing clicks on more than two cards per round.
    - Adding click functionality back after round is complete.
    - Resetting the global variables to allow for multiple rounds.
4. User can win game
    - Create global variables to keep track of the number of matches
    - Create the functionality to track the number of matches the user makes.
    - Create the functionality for the win condition to occur.
    - Build a modal which will inform the user when they have won.
    - Add JavaScript functionality to show the modal when the user wins.
5. User can view stats
    - Adding new global variables to track the number of games played, and the number of attempted matches.
    - Incrementing the attempts variable.
    - Adding IDs to the text elements which need to display updated statistics information
    - Creating a function which will display the statistics in the proper text elements at the end of each round.   
    - Adding the displayStats function call to your code so that the stats are updated each round.
    - Creating a function which will calculate the accuracy of the players attempts to match cards.
    - Updating the calculateAccuracy function for proper display of accuracy on the DOM.
6. User can reset game and play again
    - Declare a new function resetGame which will reset the statistic global variables and increment the gamesPlayed global variable.
    - Declare a new function resetCards which will remove the "hidden" class from the card-back cards so that they are no longer hidden.
    - Add a button to the modal which will reset the game when clicked.
    - Add click functionality to the new modal button which will call the resetGame button on click.
    - Add functionality to close the modal when the reset game button is clicked.
    - Add functionality to the calculateAccuracy function to fix the NaN issue.
# Bonus Features + Functionality 
7. Dynamic Card Creation
8. Card Shuffling 
