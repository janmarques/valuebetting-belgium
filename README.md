# +EV Value Sports Betting in Belgium

This document outlines some basics and lessons learned to get you started successfully sportsbetting using licensed Belgian sportsbooks.

## Introduction: what is value betting
When you and a friend each put 5 euro in the pot and then roll a die where you get the even numbers and you friend gets the odd numbers, (50% probability that you win, 2.0 odds on your money), your Expected Value (`=EV`) is 0. It is a fair game, and in the long run it is perfectly balanced and neither of you will come out ahead.

However when you each bet 5 euros, and you get numbers 1,2,3,4 and your friend gets 5,6 (66% probability that you win, 2.0 odds on your money), you have a huge advantage (`positive EV`). In the long run you will come out ahead.

Value betting is about finding those opportunities where you have an advantage (so where your win probability is too great relative to the odds on your money).

## Introduction: bankroll management
In the above scenario with 66% probability and 2.0 odds, you have found a golden opportunity. 
Say your entire bankroll is 10.000 euro (money you are willing to risk). You can choose to bet it all at once, meaning you have a 66% chance you will end up with 20.000 euro. However there is also a 33% chance you will end up with 0 euro, which is not ideal as you have no money left to bet again and chase the `positive EV`. So how much should I bet for such a great opportunity? 100, 1000, 5000?

Or a scenario where you have 1% probability, but 2500.0 odds (very unlikely chance but hugely `+EV`)?

This is where the [Kelly criterion](https://en.wikipedia.org/wiki/Kelly_criterion) comes in. It is a formula based on your bankroll, the probability and the odds and it results in an amount that is strategically optimal to bet. 

[Example 2: 1% / 2500.0](https://kellycriterioncalculator.com/?balance=10000&bookmakerodds=2500.0&fractionalbetting=1&winprobability=1) should be a 96 euro bet.

[Example 1: 66% / 2.0](https://kellycriterioncalculator.com/?balance=10000&bookmakerodds=2.0&fractionalbetting=1&winprobability=66) should be a 3200 euro bet. 

It should be noted however that there is obviously still risk involved. When you bet and lose this amount 3 times, you have pretty much gone through your entire bankroll. The probability of this happening (33%*33%*33% =~ 3%) is not extremely low. Because some people find that the Kelly criterion is a bit too agressive, they decide their own risk tolerance factor to it, and divide the suggested bet in 2 or 4 (so bet 800 instead of the suggested 3200).

