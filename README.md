## Expectations

This maven project has 3 different problems. Please focus to take these to completions. Please spend around 2 hrs to perform this activity.
It's completely fine not to complete all but please focus on design and maintainable solution rather than rushing to complete all problems

### Refactoring problem

questions.refactoring.SmallMart tries to solve following problem. Please refactor this class to make it more readable and maintainable

SmallMart is a small inn with a prime location in a
prominent city ran by a friendly innkeeper named Allison. We also buy and sell only the finest goods.
Unfortunately, our goods are constantly degrading in quality as they approach their sell by date. We
have a system in place that updates our inventory for us. It was developed by a no-nonsense type named
Leeroy, who has moved on to new adventures. Your task is to add the new feature to our system so that
we can begin selling a new category of items. First an introduction to our system:

	- All items have a SellIn value which denotes the number of days we have to sell the item
	- All items have a Quality value which denotes how valuable the item is
	- At the end of each day our system lowers both values for every item

Pretty simple, right? Well this is where it gets interesting:

	- Once the sell by date has passed, Quality degrades twice as fast
	- The Quality of an item is never negative
	- "Aged Brie" actually increases in Quality the older it gets
	- The Quality of an item is never more than 50
	- "Sulfuras", being a legendary item, never has to be sold or decreases in Quality
	- "Backstage passes", like aged brie, increases in Quality as its SellIn value approaches;
	Quality increases by 2 when there are 10 days or less and by 3 when there are 5 days or less but
	Quality drops to 0 after the concert

We have recently signed a supplier of conjured items. This requires an update to our system:

	- "Conjured" items degrade in Quality twice as fast as normal items

Feel free to make any changes to the UpdateQuality method and add any new code as long as everything
still works correctly. However, do not alter the Item class or Items property as those belong to the
goblin in the corner who will insta-rage and one-shot you as he doesn't believe in shared code
ownership (you can make the UpdateQuality method and Items property static if you like, we'll cover
for you).

Just for clarification, an item can never have its Quality increase above 50, however "Sulfuras" is a
legendary item and as such its Quality is 80 and it never alters.

### Snake Game

Please solve this using Test case described below.

Intention of the game is, Lazy snake will eat the food to grow its body. It can traverse either up/down/side ways but not diagonally in XY plane.
While eating food, it can't cut its own body. Yes. Same old NOKIA snake game !!!

 //Start a 5 X 5 Snake game. Snake will be at the center
        /**
         *       _ _ _ _ _
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *      |_|_|H|_|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *
         */
        
        //Start the game
        //Attempt move. Since food is not there, Snake will not move.
        /**
         *       _ _ _ _ _
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *      |_|_|H|_|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *
         */
 
        //Start the game
        //Place the food in 0, 0
        //Attempt move, Snake should consume the food ( 4 steps is optimal ?)

        // Before
        /**
         *       _ _ _ _ _
         *      |F|_|_|_|_|
         *      |_|_|_|_|_|
         *      |_|_|H|_|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *
         */

        // After - Body size has increased
        /**
         *       _ _ _ _ _
         *      |H X|_|_|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *
         */

      //Resume an existing game with Head (H)
        //Place the food(F)
        //Attempt move, Snake should consume the food (2 steps)
        // Before
        /**
         *       _ _ _ _ _
         *      |X X X|_|_|
         *      |_|_|H|_|_|
         *      |_|_|_|F|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *
         */

        // After
        /**
         *       _ _ _ _ _
         *      |_ X X|_|_|
         *      |_|_|X|_|_|
         *      |_|_|X|H|_|
         *      |_|_|_|_|_|
         *      |_|_|_|_|_|
         *
         */



        //Resume an existing game with Head (H)
        //Place the food(F)
        //Attempt move, Snake should consume the food (2 steps)
        // Before
        /**
         *       _ _ _ _ _
         *      |X X X|_|_|
         *      |_|_|X|_|_|
         *      |_|F|X|_|_|
         *      |_|_|X|H|_|
         *      |_|_|_|_|_|
         *
         */

        // After
        // figure out :-)
