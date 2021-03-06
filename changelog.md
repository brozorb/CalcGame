*****************************
CHANGELOG (added as of 1.8)
*****************************

2.8:
	NEW, corrupt streak powers, have an equal chance of being obtained as an epic streak power
		The two streak powers are:
			halves your timeout time
			reduces your streak by a set amount, random between 1 and your current streak - 1
	NEW, your current streak will be shown durng a game in normal or challenger difficulty.
	Bug fixes:
		issue with answer being 2 operations (div and multi) when either number = 1, so neither number can = 1 now.

2.7.3
	timing changes for ease of access

2.7.2:
	removed win-sound
	device support (in beta):
		additional devices supported, check requirements.txt

2.7.1:
	bug fixes:
		rare streak  power (timer) stacking
	balance changes:
		starting points same for all difficulty (500 x streak stacks)
		Same for gain (+ 75) and reduction (-50) x streak stacks
		common streak power(1): +10 points --> +50 points gained per correct answer
		common streak power(2): +5% points --> +15% points gained per correct answer
		rare streak power(2): +2 seconds --> +3 seconds on timeout
		epic streak power(2): +100 points --> +500 points gained per correct answer
		legendary streak power(1): Also start with double the amount of points
		legendary streak power(2): Also gain +30% points when answered correctly

2.7:
	bug fixes:
		cases of streak not resetting even when an answer is incorrect
		chance streak power not loading properly
	NEW double the amount of streak powers for each rarity (streak powers pt2):
		common = + 5% points
		rare = timer length + 2 seconds
		epic = + 100 points per question when answered correctly
		legendary = Answer only one question and gain the same as what you would of gained if you answered 5 questions
	other changes:
		now a lot more common to get a streak power but there is still a chance you wont get one

2.6.1:
	visual changes:
		updated start up instructions to be more clear.
		extended length of all leaderboards
	technical changes:
		scores and points displayed as reals so game is compatible with future updates

2.6:
	streak powers(pt1):
		chance to gain certain powers when you are on a streak above 1 and below 10
		different rarities of streak powers. The rarer it is, the more powerful it is
	bug fixes:
		critical issue with when choosing to view challenger leaderboard at the end
	Timeout changes:
		all +  1 second

2.5.1:
	reworded some text and fixed some spelling errors, for clarity
	Your streak will reset after playing a game at a streak of 10
	better input support, e.g. you can now capitilse certain inputs
	coluring for certain things changed and timing improvments

2.5:
	NEW streak feature; ths is where the longer you play games without getting an answer incorrect, the more points you gain and lose
	NEW more info about the game mechs for clarity
	bug fixes:
		Inputting an invalid input during viewing a challenger leaderboard would cause it to incorrectly displayed
		Some text being incorrectly displayed
		Some sounds never being played
	Other changes:
		can no longer change difficulty after pressing play again unlesss you were in practice mode which then causes your streak to reset
		combined two screens

2.4.1:
	NEW: view how you gained and lost your points during a game of 'normal' mode
2.4:
	more sound has been implemented as well as some being removed
	unfortunatly wav files are buggy for some reason and so can't use as much sound as i want
	slight improvements to practice mode being displayed
	changed some inputs about how they are displayed
	challenger starting difficulty is now set to 150, prev 50
	NEW seperate leaderboard for the top 5 scores for challenger difficulty
	bug fixes:
		challenger points resetting to default every time a new round is started

2.3.1:
	practice mode improvments:
		can now choose any difficulty
		looks smoother
		inputs when not prompted will be flushed
2.3:
	NEW practice mode:
		practice the game without a time limit or points
		continues forever until you end it

2.2.1:
	reworked the highscore leaderboards
	entry to the challenge now reqs 'c', prev 'challenge'

2.2:
	challenger update:
		NEW difficulty: challenger; same as hard but the timeout is 3 seconds aposed to 5, accessed by choosing hard
		Also, point value changes for challenger only:
			starting points: 50
			reduction: 30
			gain: 10
	visual changes:
		highscore leaderboard displayed better and now only displays challenger highscores (for now, changes will be made)
	balance changes:
		points (excluding challenger):
			gain: 25 --> 30
			reduction: 20 --> 25
			initial points: 100 --> 150

2.1:
	NEW: various sounds have been added
	NEW: displays the newest implemented feature at the top the first leaderboard
	balance changes:
		timings nerfed:
			easy: 7.5 --> 10
			medium: 5.25 --> 7.5
			hard: 3.75 --> 5
		number gen range changes:
			easy:
				num1: (1(min) --> 125(max)) --> (25(min) --> 100(max))
				num2: (-15(min) --> 1(max)) --> (1(min) --> 25(max))
			medium:
				num1: (max 100) --> (max 150)
				num2: (min -20) --> (min -25)
			hard:
				num1: (max 100) --> (max 150)
	ease of access changes:
		certain timings have been changed
		when timing out changes:
			Displaying 'incorrect' --> displaying 'Timed out'
	visual changes:
		spacing at welcome menu removed so whole screen can be viewed
	
2.0.1:
	bug fixes:
		spacing issue at the end when resetting the leaderboard
	ease of access:
		you can now capitalise the y / n when wanting to play again

2.0:
	Balance changes:
		Timout changes (in seconds):
			easy: 6 --> 7.5
			medium: 4.5 --> 5.25
			hard: 3 --> 3.75
		Inputing an invalid answer now removes less points; 20 --> 5
		easy diificulty values of nums can be negative now (min -10)
		modulus option removed
		the second number will now always be smaller than the first no matter the difficulty
		timeout only costs you 10 (from 20) points
	LEADERBOARD RESET; due to current high scores being unobtainable in current version
	bug fixes:
		Input buffering during sleeping no longer works
	visual changes:
		easier to read the important info during a round
		spacing change in countdown

1.9.1:
	bug fixes:
		FIXED issue with timeout timer resetting if an invaid input was inputter
		fixed by making inputtiing an invalid input will result in that question being marked as incorrect
	updated the emergency clear file to match the one ingame

1.9:
	NEW difficulty factor, timeout:
		this is where if you take too long to answer a question you will automaticly get it incorrect
		timing changes depending on difficulty:
			easy = 6 seconds
			medium = 4.5 seconds
			hard = 3 seconds
	changed the start up instructions to be more presentable
	points gained and reduced are now fixed at:
		gain = 25
		reduction = 20
	certain timings for displays have been balanced

1.8.4:
	balances:
		'hard' and 'medium' difficulty more balanced
1.8.3:
	Wiped leaderboard change (for scores): 1 --> 0
	added correct answer to be shown when an answer is incorrect

1.8.2:
	changed colour scheme for highscore leaderboard
	bugs fixed:
		spacing issue in-game
		colouring issue in leaderboard

1.8.1:
	number of rounds set to 5 (from 10)
	coloured wiping of leaderboard
	added emergency wipe incase of an issue to arise

1.8:
	coloured update:
	added colour to almost everything:
		colours include: yellow, magenta, cyan, blue, red and green
	starting points now fixed at 100 (from between 90 and 120)
	point randomness reduced:
		reduction (15,25) --> (15,20)
		gain (15,25) --> (20,25)
0
