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
Now, you have better things to do than to check all those 100s bookmakers yourself, calculate the averages, etc... . This is where a service like [surebet.com](https://en.surebet.com/valuebets) comes in. They have real-time access to all kind of odds across very many bookmakers. Based on that information, they can calculate the fair prices and single out the bookmakers and odds that are `+EV`. Best thing is that this site is entirely free for now. So go ahead and create an account there.

### Using surebets.com
On the valuebets page on the right, you can see a bunch of filters. Let's start out by picking our bookmaker. When the popup is open, on the bottom right you can uncheck all the bookmakers at once. Then search for `Circus (BE)` as an example, because this will work out of the box. Put the Probability at 0 and the Overvalue at 0 as well.

Now you should see a whole list of all the bets that `Circus` offers that are actually `+EV`. 

When you click on the probability percentage for a certain bet, a page will open that shows all the other bookmakers that have that same bet, with their own odds. This is a nice way to get a closer feel of how the system works behind the scenes (gathering the average odds). **Sometimes surebet.com will also make mistakes itself, and compare multiple odds that are not actually of the same event. That's why it is a good idea to check this page and manually verify that the event titles actually match and the same bets are being compared.**

When you click on the event name of the bet (for the `Circus` bookmaker), you will be redirected to the event on `Circus`es website. There you should search for the exact bet, verify that the odds are indeed the same as advertised, and then place your bet. For the amount you bet, use the Kelly criterion as explained earlier.

## Configuring the filters
Previously, we had set the probability and overvalue to 0, to make sure there were bets available for we could continue the guide. It is however advised that we tweak these a bit.

### Probability
In the long term for `+EV` bets, your probability can be set to 0 and in theory it does not matter. However if you are starting out and you place 10 bets that each have a 1% chance of winning, you will very likely just lose them all, even if they are all `+EV`. So just psychologically, it is interesting to set the minimum probability to `50%` when starting out.

### Overvalue
This is the extra margin that the bookmaker odds give you over the fair odds.
Anything over 0% is `+EV`, but given that you only have a certain amount of money to invest, most people set this to at least `3%`. It is also advised to sort by overvalue, so you make your most valuable bets first, and move to less valuable bets only with money left over.

### Minimum odds for calculation
This determines how many bookmakers have to offer the bet in order to calculate the fair odds. The more bookmakers there are, it is likely that the calculation will be more accurate. Advised to set to `50` to start out, but can be lowered if you're having trouble finding bets.

### Sports
This determines for which sports the bets are shown. It is advised to disable the `Virtual sports` as well as the `E-sports` that correspond with a real sport (like `E-Football`). This is because surebet.com will sometimes mix up events across those categories. (Personally I also suspect some bookmakers to take advantage of this and purposfully schedule their virtual sport along with an E-Sport so people accidentally bet on the wrong one.) If you want to bet on this anyway, carefully check the odd details across the different bookmakers.

### Event time
This determines how far out you want to place your bets. With a very large bankroll, you can set this as far out as you want, as you will have the money to make any bets you want. 

With a smaller bankroll however, it is advised to place bets that will resolve quite quickly. If you place a bunch of bets on events that resolve next week, you have no money left to place event in the meanwhile, and your money is not 'working'. So while 10% bet that resolves in 7 days is good, it is far more interesting to place 7 times an 8% bet that resolves the next day each time. So start with `2 days` on a smaller bankroll.

**Betting volume really is the name of the game.** Notice that your total expected profit is `Volume * overvalue percentage`. So if during a week you can bet your 1.000 completely every day, your volume will be 7.000. Sometimes you can even try to go faster with this, and bet your money more than once a day.

## Bookmakers
When selecting the bookmakers, you will notice that surebet.com does not list that many known Belgian bookmakers. However our Belgian bookmakers are often part of a multinational or use the same software, meaning that you can use other bookmakers to get the odds that will be the same on a different site. 
([List of officialy licensed sportsbooks](https://www.gamingcommission.be/en/gaming-commission/legal-games-of-chance/betting-shops-online) )

|Surebet bookmaker|Belgian bookmaker|Notes|
|---|---|---|
|Circus BE|Circus-sport.be|Gaming1 software|
||blitzbet.be|Gaming1 software|
|Goldenvegas BE|goldenvegas-sport.be|Gaming1 software|
|Bet777|bet777.be|Gaming1 software|
|| 
|Bingoal|bingoalsport.be|Kambi software|
||unibetsports.be|Kambi software|
||scooore.be|Kambi software|
|| 
|Campeonbet|starcasinosport.be|Altenar software|
||goldenpalacesports.be|Altenar software|
|| 
|Eurobet|ladbrokes.be||
|BetFirst (BE)|betfirst.dhnet.be||
|1xbet|vivatbet.be||
|Superbet|napoleonsports.be||
|Betcenter (BE)|betcenter.be||
|Zebet (BE)|zebet.be||
|Meridian (BE)|meridianbet.be||
|Bwin (BE)|bwin.be||
|?|magicbetting.be|Exists but not found|
|?|eurotierce.be|Not found|
|?|bet90.be|Not found|
|?|betanosports.be|Not found|
|StanleyBet (IT)|stanleybet.be|Untested|

## Remarks


### Getting limited
The sportbooks obviously do not want winners on their site. It will take some time for them to confirm that you are indeed a winning player, but once they do, they will limit your action. Meaning that you can bet either lower stakes only, or nothing at all. At this point you should withdraw your money and move to the next bookmaker. 

Also note that some bookmakers that run the same software, will likely share your player profile between their different sites behind the scenes. Meaning if you are limited on for example `Circus`, you may also become flagged on `blitzbet` and get limited there faster.

Therefor it is advised that you take your first small steps on an independant bookmaker (not linked to any other ones) and familiarize yourself with the betting procedures. Once you get limited there, you can move to a different bookmaker and you will be a completely unknown person there.

Later on in your career, with a large bankroll, it may be a strategy that you hit and run all bookmakers of the same software at the same time. This way you can get your bets in at the various sites together, before they are able to flag you as a winner. Of course you still need to play within your bankroll means.

### Opening an account, deposit, withdraw, KYC
To open an account on any bookmaker is very easy. Usually in a couple of clicks along with your itsme. Also depositing is insanely easy with a lot of options. They want to get your money as fast as possible. Notice that due to Belgian law, you are by default only allowed to deposited 200 euro per week. If your bankroll is bigger and you want to deposit more, you can ask to have your limit increased (this will typically be linked on the deposit page). There is a couple days wait period for this. If you plan on making big bets, it may be advised that your first get your big deposit in and then place the big bets. Rather than making some small bets with the 200 in the meanwhile, because they may already be help the bookmaker in determining that you are a winning player and getting you limited.

When withdrawing your winnings however, a lot of the bookmakers will make you jump through many hoops. Even they already have your ID through itsme, they will try to delay you by asking for selfies, bank statements, utility bills etc (called Know Your Customer or KYC). This is a tactic to attempt that you don't do it, so they can just keep your money. So be prepared to do this and stick to it, even though it is bit annoying.

### Fake / duplicate accounts, family member accounts, ...
It is strongly advised not to use a fake account. For any substantial amount you win, they will probably do a thorough KYC check and find you out. They may not pay out nor refund your initial deposits.

Similarly for using an account of a family member: most bookmakers say in their Terms of Service that there can only be one account per household. So they may be able to fingerprint your device, use your ip-address, ... .

Opening these accounts and placing bets won't be an issue, but you may run into serious issues when trying to cash out.

### Unlicensed bookmakers / crypto bookmakers

### Bet choice (betting the same outcome)
#### Not too little
On most bets, there is always a limit of how much you can bet. If you want to bet 500 on `team A` winning, but you are only allowed to bet 300, you still have 200 left. Perhaps surebet also suggest you can bet on `team A or a draw`, and you can bet the remaining 200 there. This way you are betting closely related events, but spreading them.

#### Not too much
Inversely, if you made your desired 100 bet on `team A`, it may not be wise to also bet 100 on `team A or a draw`, because they are very closely related, and you are pretty much betting 200 on `team A`, while you only wanted 100 in exposure. (Not exactly correct of course, but to illustrate the point).

On the other hand, if within the same match you want to bet on who wins, and who has the most yellow cards, and the most offsides, these events are less closely related so can be deemed to be not cummulative in exposure.