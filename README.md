# Elevens-Lab-Activity7

1. What items would be necessary if you were playing a game of Elevens at your desk (not on the
computer)? List the private instance variables needed for the ElevensBoard class.

	You would need a deck of cards in order to play eleven not at your computer and a 	surface to put the cards and deck on. The private instance variable needed are 		cards, deck, suits, ranks, and point values.

2. Write an algorithm that describes the actions necessary to play the Elevens game.

	basically pick two cards in the dealt cards and if they equal up to 11 then 		replace those cards with two other in the deck and decrease the size of the deck 	by 2 and don't allow those 2 cards to be dealt again. If a king, queen, and jack 	are pulled and all selected, then take those out of the dealt cards and put 3 new 	cards in from the deck and decrease the size of the deck by 3 and don't allow 		those three cards to be drawn again. If two cards are selected that do not add up 	to eleven, do nothing. If more than two cards are selected and are not a king, 		queen, and jack only, return nothing. If no cards in the dealt class in the dealt 	cards add up to 11 or if there are no king, queen, and jacks on the board, end 		game and return "sorry, you lose." If all cards are selected and replaced until 	there is an empty deck and the rest of the dealt cards are selected, print out 	"you win!"

3. Now examine the partially implemented ElevensBoard.java file found in the Activity7
Starter Code directory. Does the ElevensBoard class contain all the state and behavior
necessary to play the game?

	No the code is missing methods to see if there are any matching pairs, determining 	whether or not another move is possible

4. ElevensBoard.java contains three helper methods. These helper methods are private
because they are only called from the ElevensBoard class.

a. Where is the dealMyCards method called in ElevensBoard?

	it is called in the ElevensBoard constructor and the newGame method




b. Which public methods should call the containsPairSum11 and containsJQK
methods?

	isLegal should call both methods



c. It’s important to understand how the cardIndexes method works, and how the list that it
returns is used. Suppose that cards contains the elements shown below. Trace the execution
of the cardIndexes method to determine what list will be returned. Complete the diagram
below by filling in the elements of the returned list, and by showing how those values index
cards. Note that the returned list may have less than 9 elements.

![My image](https://bsimps3.github.io/Elevens-Lab-Activity7/cards.png)

	returned list will return in this order J,6,2,A,4 and will only go up to index 4

d. Complete the following printCards method to print all of the elements of cards that are
indexed by cIndexes.
    public static printCards(ElevensBoard board) {
    List<Integer> cIndexes = board.cardIndexes();
    	System.out.println(cIndexes);
  
  
  
    }
  
  
  e. Which one of the methods that you identified in question 4b above needs to call the
      cardIndexes method before calling the containsPairSum11 and containsJQK
      methods? Why?
		
		The List method so it can establish cardIndexes as being equal to 			cIndexees.









