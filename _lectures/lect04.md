---
num: "Lecture 04"
lecture_date: 2022-04-06
desc: "Wed Section: Happy Cows, jpa01, jpa02"
ready: false
---

# Today

* Start playing Happy Cows
* Work on jpa01, jpa02

# Use `#help-lecture-discussion` 

During lecture and section, if you need help with anything, please use the `#help-lecture-discussion` channel.  We use this as a "help queue" to try to make sure that we get to all of the questions asked in the order in which they were posted.

# Start Playing Happy Cows

Last quarter (W22), the students in CMPSC 156 worked on two applications:
* Courses Search (a new version of this web page <https://my.sa.ucsb.edu/public/curriculum/coursesearch.aspx>
* Happy Cows, a simulation game used in CHEM 123

Last year's CHEM 123 class used an older version of the game written in a different web framework.   
* That implementation had some serious performance issues, due to some inefficient coding.
* We'd like to try to understand those performance issues a bit better
* And, we want all of you to understand the game a bit better.

So, we are going to actually *play the game* for a couple of weeks.

# About the game

* In the game, you are a farmer.  The object of the game is profit. (You need this profit to feed your family.)
* You start with a certain amount of money with which you can buy cows.
* You can buy cows or sell cows at any time.
* If you have cows, they get milked every day at 5am, and you get profit.
* But all of the cows share a common grazing area.  If there are too many cows, they start to get sick, and produce less milk.
* Eventually, if the cows get too sick, they may die.
* So, if cows start dying, you may want to sell off some cows in order to let the herd recover.

You can check on your cows once a day.

# How do I join the game?

Joining the game will count as a participation activity, P04.

1. Navigate to: <https://chem123.chem.ucsb.edu/>
2. There is a shared username and password to get to the next screen; it will be shared on the slack in the `#happycows-game` channel.  Please keep these shared credentials confidential within student in CMPSC 156 S22.
3. Once you are past that screen, you'll be asked to login with an OAuth username/password; you can use your UCSB email here.
4. You should then see this page:

   <img width="1111" alt="image" src="https://user-images.githubusercontent.com/1119017/162081355-bb9430cd-f516-4c69-b641-f50a54b6c23f.png">

   Each of the "Commons" listed on the right hand side of the screen is one instance of the game.
   
   Please click where it says "Join Commons" beside two of the commons: 
   * Everyone join the one called: `cs156-s22`
   * Everyone also join the one corresponding to their discussion section, either `cs156-s22-4pm`, `cs156-s22-5pm` or `cs156-s22-6pm`.
   * Please do not join any other game.

   The different games have different parameter settings for the price of a cow, the price of milk, and the number of players.  We are hoping to learn about how these different parameter values affect game play, and game performance.
   
5. Once you join a commons, the games you have joined will appear on the left hand column, like this:
   
   <img width="1118" alt="image" src="https://user-images.githubusercontent.com/1119017/162081889-a6c24c7a-de95-4e27-b563-dde036a15373.png">

   You can click the "Select" button to visit any of the commons (farms).   When you visit a farm, look to see how much money you have and
   decide whether you want to buy any new cows or not:
   
   <img width="1138" alt="image" src="https://user-images.githubusercontent.com/1119017/162082048-f9ab7020-5919-4775-a0c6-8c06cd1b3124.png">

   This is what it looks like after one day; I started with $1000 and purchased nine cows.  That left me with $100.  Then, after one day, I had earned $18 additional dollars; $2 for each of my nine cows.  At this point, the cows are all in good health, it would appear.  But perhaps as more cows are purchased, that may change; we'll see!   
   
   Also: the price of a cow may be different for each of the different sections; and we may change the prices over time.
   
Once you've joined the games for both your section and for the class as a whole, please make a post on your team channel on Slack indicating that you joined the game.   Then you can turn to working on jpa01, or jpa02.

# Working on jpa01 and jpa02

If you have questions about either of these, use `#help-lecture-discussion`.

You may also want to check `#help-jpa00`, `#help-jpa01`, and `#help-jpa02` to see if there is any new information that may be helpful to you.

* jpa01: <https://ucsb-cs156.github.io/s22/lab/jpa01/>
* jpa02: <https://ucsb-cs156.github.io/s22/lab/jpa02/>

