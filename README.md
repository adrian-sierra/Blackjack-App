Blackjack Web Application


Simple blackjack game that utilizes HTML, CSS, and vanilla Javascript, and can be ran using a Live Server extension on Visual Studio Code, after all files and images are downloaded.

The application utilizes objects to store the data for each card in a normal deck of cards. Each object corresponds to a number, as a string, between 1 and 52, and each card has three attributes: name, value, and a card image.

The game is set up for one player playing against the dealer and each one is handed two random cards to begin the game. Just like the actual game of 21, if either player starts off with a hand that has a value of 10, the power cards, and an ace, then that player will win the game automatically. If no one wins the game off of the first two hands dealt to each, then each player is able to click the "Hit" button to add one card to their hand, and the game is won if a player gets 21, or if the other player has a hand that adds up to over 21. The players are then able to press the "Start Over" button to refresh the game and play from the start, with two new random cards.

The internal functionality of the application is that each player is associated with an array, which holds the value of the card that is associated to them. When the card is associated to the corresponding player, internally, there is a random number between 1 and 52 that is generated and then that number is utilized as the key to get the corresponding attributes of that number card. Once that card's attributes are retrieved and associated accordingly, then that key and corresponding card is deleted from the object data structure and can no longer be drawn for either player, therefore, there is a single deck that is utilized with each game. And on each passing "Hit" button click, we add the value of the card to the array associated to the player and passed to a function to get the total of the array, and the corresponding event occurs as a result of the total, as explained above.

The JavaScript aspect of the application is simple and involves simple DOM manipulation, given the action of clicking on the various buttons on screen, and the displaying the appropriate value of each player, the appropriate card that is drawn, and then the winning player display.
