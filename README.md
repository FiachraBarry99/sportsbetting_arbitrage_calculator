# Sportsbetting_Arbitrage_Calculator
This python script creates two functions, one to calculate if an arbitrage opportunity where bets are placed on all possible outcomes is profitable and another to calculate if an arbitrage oppurtunity where a bet is placed on one site and then the corresponding bet is layed on an exchange.

### Functions and Arguments

- back_lay (back_stake, back_odds_matrix, lay_odds_matrix)
	- back_stake = the amount to be placed on the back betting site
	- back_odds_matrix = a matrix/array with all back odds
	- lay_odds_matrix = a matrix/array with the lay odds

- arbitrage (total_stake, back_odds_matrix)
	- total_stake = the total amount that will be placed
	- back_odds_matrix = a matrix/array with all back odds
	
	
### Odds Matrices Formats

> back_odds_matrix = numpy.array ([ [awins0, awins1, awins2,....awinsn], [draw0, draw1, draw2,....drawn], [bwins0, bwins1, bwins2,....bwinsn] ])

> lay_odds_matrix = numpy.array ([ [awins], [draw], [bwins] ])

At the moment the script is configured so that the 0th bookie is Betfair Exchange, the 1st bookie is Unibet, the 2nd bookie is William Hill and the 3rd bookie is Paddy Power. Though this could be easily changed to different bookies or to include more or less bookies. Also the script can only take in one bookie for lay odds but again this could be changed.
