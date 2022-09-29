an Ugly Trivia Game

This game needs refactoring!

Two things to consider:
1. Testing with Golden Master

We can’t write reasonable unit tests without refactorings first. But we don’t want to refactor without tests at all.

But we can test the application as a whole. Gain control over all external input sources (RNGs, system time, keyboard input and so on). Then save all outputs produced (console output, emails sent, files changed etc). This is our Golden Master.

Now we can change the code and compare if it still yields the same results as before.

2. Using Tools - Free Fall

This is another thing to try out. And probably it’s a good idea to not learn this in production. Just use your IDE refactorings. Do not waste time to understand the code. Trust your IDE and use features like extract method or invert if statement. You will be surprised about the results.

The trivia Game is an automated game where players are added and are given questions. Based on the spots their are on the board(just numbered spaces from 1-10), they get the question right or wrong and the board also determines their type of question. if they get it right, they get a coin. if they get it wrong, they go to the penalty box where the must roll an odd number to get out. to win, a player needs 6 coins. 

I have organized this so that there are a few main function sections: adding a player, rolling, detemining whether they are right, and add point or penalty house. Under these sections, there are other functions to help cleann up these larger functions. 
