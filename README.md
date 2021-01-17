# Sportsbetting_Arbitrage_Calculator
This python script creates two functions, one to calculate if an arbitrage opportunity where bets are placed on all possible outcomes is profitable and another to calculate if an arbitrage oppurtunity where a bet is placed on one site and then the corresponding bet is layed on an exchange. At the moment it is only possible to lay a bet on one exchange/site. The functions and arguments are as shown below: 

- back_lay (back_stake, back_odds_matrix, lay_odds_matrix)
	- back_stake = the amount to be placed on the back betting site
	- back_odds_matrix = a matrix/array with all back odds
	- lay_odds_matrix = a matrix/array with the lay odds

- arbitrage (total_stake, back_odds_matrix)
	- total_stake = the total amount that will be placed
	- back_odds_matrix = a matrix/array with all back odds
	
	
The odds matrices are formatted as follows: 

> back_odds_matrix = numpy.array ([ [awins1, awins2, awins3,....awinsn], [draw1, draw2, draw3,....drawn], [bwins1, bwins2, bwins3,....bwinsn] ])

> lay_odds_matrix = numpy.array ([ [awins], [draw], [bwins] ])
