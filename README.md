# BlackJack

Design a python program to play Blackjack Game!

Using Functions & Classes

    1.Create a deck of 52 cards
    2.Shuffle the deck
    3.Ask the Player for their bet
    4.Make sure that the Player's bet does not exceed their available chips
    5.Deal two cards to the Dealer and two cards to the Player
    6.Show only one of the Dealer's cards, the other remains hidden
    7.Show both of the Player's cards
    8.Ask the Player if they wish to Hit, and take another card
    9.If the Player's hand doesn't Bust (go over 21), ask if they'd like to Hit again.
    10.If a Player Stands, play the Dealer's hand. The dealer will always Hit until the Dealer's value meets or exceeds 17
    11.Determine the winner and adjust the Player's chips accordingly
    12.Ask the Player if they'd like to play again


Step 1: Import the random module. 

        1. This will be used to shuffle the deck prior to dealing. 
        2. Then, declare variables to store suits(list), ranks(list) and values(dictionary). 
        
Step 2: Create a Card Class

        1. A Card object only needs two attributes: suit and rank. 
        2. add a _str_ method to the Card's init method to print a Card and format the output, returns a string in the form "Two of Hearts" 
        
Step 3: Create a Deck Class. Here we store 52 card objects in a list that can later be shuffled. 
        
        1. First, we need to instantiate all 52 unique card objects and add them to our list. 
        2. build Card objects inside our Deck init method. 
        3. iterating over sequences of suits and ranks to build out each card. 
            (for suit in suits: for rank in ranks)
        4. In addition to an init method, add shuffle() method to shuffle the deck.

TESTING: Just to see that everything works so far!

Step 4: Create a Hand Class

        1. add method used to add a card to the player or dealer' hand, when adding to their hand, then remove a card from the deck
        2. get_value method is used to calculate the value of those cards using the values dictionary defined above. 
        3. It also need to adjust for the value of Aces when appropriate.
        4. getHand method to return the cards in each players' hand.
        
Step 5: Create a Chips Class
        
        1. write methods to add chip, subtract chip and return the chip on hand.
        
Step 6: Write a Bet() function for taking bets

        1. use try/except to control the input from the user.
        2. check that a Player's bet can be covered by their available chips by using a WHILE loop.
        
Step 7: Write a Hits() function for taking hits

        * Either player can take hits until they bust. 
        * This function will be called during gameplay anytime a Player requests a hit, or a Dealer's hand is less than 17. 
        * It take in Deck and Hand objects as arguments, and deal one card off the deck and add it to the Hand. 
        
Step 8: Write a HitOrStand() function prompting the Player to Hit or Stand
        
        1. This function accept the deck and the player's hand as arguments 
        2. assign playing as a global variable. 
        3. If the Player Hits, employ the Hit() function in step 7. 
        4. If the Player Stands, set the playing variable to False - this will control the behavior of a while loop later on in the code.        
     
Step 9: Write Display() function to display cards

        When the game starts, and after each time Player takes a card, the dealer's first card is hidden and all of Player's cards are visible. At the end of the hand all cards are shown, and show each hand's total value. 
        
And now on to the game!!


Thank you!
        
        
