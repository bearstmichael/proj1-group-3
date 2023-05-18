# proj1-group-3

# Analyzing NBA Shot Data #
### Bear, Naveen, Jake, Noah ###

## Data Description ##
We are analyzing NBA's 2014-15 season, with some focus on the 76ers in particular. We drew this data from Kaggle.com, which contained datapoints for each attempted shot in each game that season, along with properties of that shot, such as distance, success of shot, closest defender, time on shot clock, and time of game. This dataset had 21 columns and 128,069 rows.

## Analysis ##
*Question 1:* Which players on the 76ers in the 2014-15 season were the most effective defenders?

*Figure 1:*

![bear_homeaway_splits](https://github.com/bearstmichael/proj1-group-3/assets/128632655/a9305f2a-afca-4d01-ae8a-001e387f98cd)

This chart is designed to present offensive production ( number of points from 2’s and 3’s, no free-throws). It splits it into their average production at home vs away. It tracks all players for the 76ers in this season, qualified based on having made at least 4.0 shots per team game.

The common assumption is that playing at home is a general positive influence. But really it depends on the player. Some players generally improve (e.g., Robert Covington), other players generally worsen (KJ McDaniels). Some just change the amount of points they get from 2’s vs 3’s, without much change to the overall total.

This chart demonstrates whose performance is impacted the most, based on home-away splits. Some have large negative effects (e.g., KJ McDaniels), some have large positive effects (e.g., Robert Covington). Some are consistent whether they’re home or away (e.g., Hollis Thompson). That said, consistency is only extra special if you’re consistently good, and averaging ~7 points per game is not particularly good.

It’s interesting to point out that you don’t necessarily want a bunch of long arrows pointing to the upper left corner, because that would suggest that everyone is worse at home. Ideally you want shorter arrows, implying consistency whether home/away. Or, you want at least everyone’s arrows to be pointing in different ways, to different extents, such that they all balance each other out, yielding an overall consistent performance at home or away.

An interesting step way to go with this analysis would be to compare this with the chart for another team, or instead to look at home-away splits for whole teams, instead of players.


*Question 2:* Which players on the 76ers in the 2014-15 season were the most effective defenders?

*Figure 2a:*

![bear_twopt_defense](https://github.com/bearstmichael/proj1-group-3/assets/128632655/a1fd0d77-2084-4f2f-a3be-09cd603eec0e)

This chart shows the shooting Success Rate Against for qualified defenders on the 76ers. Here, qualified means that the player has had at least 4.0 defensive opportunities per team game. Here, I am defining a “defensive opportunity” as a player being the physically closest defender on the course when the shot is taken.

This Success Rate Against is calculated as the percentage of 2-pointers attempted that are actually made. So as a defender you want a low Success Rate Against. For comparison, I have included the 2014 Defensive Player of the Year, Kawhi Leonard. You’ll note that there isn’t actually very much difference between players.

*Figure 2b:*

![bear_tript_defense](https://github.com/bearstmichael/proj1-group-3/assets/128632655/3679549a-bc40-429e-a322-62344cc1a93c)

When we look at 3 pointers, we see that the overall shot success rate goes down, which makes sense because 3 pointers are more difficult shots. But we see again, that there isn’t much variation between players.

From this, we can conclude that all of the players on the 2014-15 76ers we as good as Kawhai Leonard! … or we can deduce that shooting Success Rate Against isn’t a particularly valid metric of defender impact. It requires that the shots are still taken, which an effective defender would mitigate, and it assumes that the closest defender is the most impactful, when in fact effective defenders are effective at least in part because they are in high leverage positions keeping the opponent away from high leverage shooting opportunities.

I was definitely surprised at how uninteresting the surprises were, but at least we learned something about a stat that is *not* that useful. But we still learned something about our dataset, in terms of what conclusions we could, and could NOT, draw from it.


*Question 3:* 
*Figure 3:*


Noah Analysis

Slide 1: For the 76s what is the mean points earned per period?

![image](https://github.com/bearstmichael/proj1-group-3/assets/128091997/45b6c4d5-3c7a-4b59-91b9-a074a61dade6)

We must put this question into the context of the whole season, How were the 76s preforming that season? Not well. They would win 18 games and lost 64
What did the 76s look like on game day? While usually starting off strong if the 76s did not have a good 3rd period there game was over. The ability to put up a modest amount of points in the second period and match those points in the 3rd was the ultimate predictor of winning or losing. 
You could also conclude that the game could be predicted by the first period alone. When the team won a game, their lowest scoring period (4th) would earn them more points than their highest scoring period (1st)during a loss. This means that if the team scored close to 15 points on the first period it was extremely unlikely that they would win. 

Slide 2: How did the points earned by 76s players stack up to rest of the league?

![image](https://github.com/bearstmichael/proj1-group-3/assets/128091997/df4d4253-1cfb-482c-b32b-b5a052e4b656)

Continuing the idea of putting the numbers into the context of the season, it is clear the 76s could not perform well. The average player earned 454 points during the 2014-2015 season. The closest a 76s player came to this is Michael carter Williams with 235.
The end goal of basketball is to score more points than your opponents. Considering the extremely low volume of points the 76s were able to score it is no wonder they only won 18 games their whole season.


