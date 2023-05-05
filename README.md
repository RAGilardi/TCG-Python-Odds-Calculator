# TCG-Python-Odds-Calculator
This small project was born as a simple self-assignment, with which I tried to use Python (mostly scipy.stats) to recreate a "Trading Card Game odds calculator", by which I mean an instrument with which to calculate the probability of drawing any amount of copies of a certain card, or a combination of cards, from a deck.

There are already NUMEROUS of these calculators online, most of which don't show their source code behind the GUI. I just tried to build the logic from the ground to review some of my knowledge in statistics and explore a bit of Python libraries I hadn't already used.

In particular, there are two main sections in the notebook:
- A **"Copies Drawn" calculator**, which shows the odds of drawing any number of copies of a card from a deck
- A **"Combination Drawn" calculator**, which tells the odds of drawing multiple cards in the same hand

The code is free to use and it is almost completely a direct use of already available functions, simply adapted for this particular problem.

The results should all be correct and have been compared with other calculators'.

The function used in this program could be used to build software that calculates the odds of drawing a certain card during a game (such as Untapped Companion: https://mtga.untapped.gg/companion), but as this could be considered cheating I explicitly maintained my code focused on the deckbuilding side of odds calculation.

As I am myself a Magic the Gathering player (https://magic.wizards.com/en), most of the examples below will use MTG vocabulary, but the code can be used for any kind of situation with a "deck" and "draws".

**EDIT 04/05/2023:** After almost completing the code, while I was looking for some different calculators with which to compare my results, I found another one explicitly talking about hypergeometric distribution and multivariate (hypergeometric) distribution as mine: https://www.mtgnexus.com/tools/drawodds/. This also gave the same results as my code, which I believe is enough proof that the calculations are accurate. 

In the case of the combination calculator, I yet didn't find a calculator which can work with any number of cards like mine.

**EDIT 05/05/2023:** In the end of the notebook I also **added** an **extra section** about a better implementation of the iterative code used in section 2 based on an answer I received to a question on stackoverflow, which showed me some tech I didn't know and I tried to implement myself with the functions I originally used.
