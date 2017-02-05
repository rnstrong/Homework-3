206 Project 1 - Code for playing cards
README

Your name: Renee Armstrong
Anyone you worked with: N/A

----- 


This code is intended to create an automated and altered game of War between two players. It does this by creating cards for decks and hands for players. This code is a good example of how classes work and can be used as a teaching device and example for students.


Class Descriptions:
Class Card (line 4):
	This class represents a single card with a suit (Diamonds, hearts, Spades, or clubs) and a rank (1 through 13) attached to it. It also contains the rank equivalencies for face cards (ace, jack, queen, king). 

	To create a card, a suit and rank should be assigned. 

	There are only two methods in this class, the init and the __str__ method which create a Card instance and give the written description of the instance (i.e. "Ace of Hearts") respectively.

Class Deck (line 20):
	This class represents a set (a list) of 52 Card instances that reflects a standard deck of cards in the real world. 

	There are no required inputs to create a deck of cards.

	Methods:
		Constructor: Creates an instance of class Deck and does not require any input

		pop_card: This method removes the last card in the deck (by default) and returns that card. You can choose to input a card (a number representing its place in the deck) and it will remove and return that card instead.

		shuffle: Randomly changes the order of the cards in the deck and requires no input

		replace_card: This method checks a card against the deck and if that card is missing from the deck, then it puts it back in to the deck. This method requires you to input an instance of class Card. 

		sort_cards: This resorts the deck in a standard way (aka the way it was organized when it was first created)

		__str__: Does not require any input and is the string representation of the class instance (a mulitline string of all the cards in the deck) it is called on

Class Hand (line 64):
	An instance of this class represents a hand of cards for the game.

	To create an instance of this class, you must have the deck you would like to use and the number of cards
	as input.

	Methods:
		Constructor: creates an instance of class Hand and requires the deck and number of cards desired as input

		place_card: Same functionality as pop_card above but for the hand instance instead of the deck. So, removes the last card (by default) and returns that card from this method.

		get_suits_available: Returns a list of all the suits that are in the hand

		get_ranks_available: Returns a list of all the ranks that are in the hand

		specific_card: input a suit and rank and if that card is in the hand, remove it from the hand and 
		return it with this method. If the card is not found, return None.

		add_card: Requires a card instance as input. Adds a card to the hand if there is not identical card already there. 

		__str__: Does not require any input and is the string representation of the class instance (a multiline string of cards in the hand) it is called on.




