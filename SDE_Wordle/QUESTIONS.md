# Reflection Questions

Answer these questions thoroughly after completing the assignment, using examples from your code. Good answers will be 1-2 paragraphs that cite specific code examples and show a meaningful reflection on how your development went, and how it could be improved in the future.

## Question 1

 In the Black-Box testing for GameState.submitGuess() portion of the assignment, list the partitions of inputs and fields that you used for your test plan. Cite specific tests by name and line number that cover each partition. A bulleted list is acceptable here. You should include all of your tests covering at least one partition. Additionally, for each partition, label it is equivalence, boundary, or exception.

## Answer

* correct answer no caps (line 10 - getLetterResults_correctAnswer(), equivalence)
* correct answer w/ caps on guess (line 50 - getLetterResults_correctCapitals(), equivalence)
* correct answer w/ caps on (line 58 - getLetterResults_correctcapitals2(), equivalence)

* repeated letter in guess where there is only one in answer (line 18 - getLetterResults_repeatLetters(), equivalence)
* no letters in common (line 26 - getLetterResults_allWrong(), equivalence)
* no repeated letters, no correct letters, just letters in wrong spot (line 34 - getLetterResults_noRepeatsWrong(), equivalence)
* no repeated letters, some correct letters, letters in wrong spot (line 42 - getLetterResults_noRepeatsWrong2(), equivalence)

* test throws exception for guess (line 66 - getLetterResults_invalidArg(), exception)
* test throws exception for answer (line 71 - getLetterResults_invalidArg2(), exception)

## Question 2

The function submitGuess(String) in WordleGameState can throw two different Exceptions. Why would we as developers intentionally design our program to throw Exceptions? What is the benefit?

## Answer

As developers, we make our program throw exceptions like GameAlreadyOverException and IllegalWordException so we can handle unexpected or bad situations in a clear and controlled way. Using exceptions helps keep the program from going on when it’s in a state it shouldn’t be. For example, GameAlreadyOverException makes sure players can’t keep guessing after the game’s already done, and IllegalWordException stops guesses that aren’t valid words. This helps keep the game working right and stops errors from messing things up.

Also, throwing these specific exceptions makes fixing problems easier because you know exactly what went wrong. Instead of some confusing, general error, you get an exception that tells you the issue right away. It also makes developers write better code by handling errors instead of just letting the program crash when something bad happens.

On top of that, exceptions help make things clearer for both developers and users. When something goes wrong, a well-named exception with a good message helps everyone understand what the problem is and how to fix it. Using special exceptions like GameAlreadyOverException and IllegalWordException is good design because it keeps the errors clear and focused. In the end, having exceptions like these makes sure the program stays solid, is easier to fix, and gives better feedback when things break.
