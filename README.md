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

# `+EV` sportsbets
Let's use `Paul vs Tyson` as an example. There are 100s of bookmakers around the world. When you check all their odds on Paul winning, let's say that the average odds you get across those bookmakers is 1.5. Of course the bookmakers also take their own margin (called [vigorish](https://en.wikipedia.org/wiki/Vigorish)), so let's say that the real fair odds on Paul winning are actually 1.6. (While the bookies only pay out as if it were 1.5, so they make their profit in the long term from that 0.1 odds difference.) This is the way we will be determining the probability of the outcome of a bet. We don't know or care about each fighters intrensic strength / form / matchfixing / ... . We just assume that all the bookmakers put together have a fair view on what the true probability is.

Now all that is left, is finding a bookmaker that will pay out more than what the probability dictates. Say that Unibet offers 1.8 odds on Paul winning. They are greatly underestimating that Paul would win. So they would pay out 180 euro instead of the 150 euro that the average bookmaker would. More importantly, it is also greater than the 'fair' price where you take away the bookmarker margin, which would payout 160 euro. This 20 euro difference between the fair price and the price of the bookmaker you found is where the `+EV` lies. While of course you can still easily lose this bet, if you place many similar of these bets you should be expected to win.

## Finding `+EV` sportsbets
Now, you have better things to do than to check all those 100s bookmakers yourself, calculate the averages, etc... . This is where a service like [surebet.com](https://en.surebet.com/valuebets) comes in. They have real-time access to all kind of odds across very many bookmakers. Based on that information, they can calculate the fair prices and single out the bookmakers and odds that are `+EV`. Best thing is that this site is entirely free for now.