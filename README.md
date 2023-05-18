# proj1-group-3

# Analyzing NBA Shot Data #
### Bear, Naveen, Jake, Noah ###

## Data Description ##
We are analyzing NBA's 2014-15 season, with some focus on the 76ers in particular. We drew this data from Kaggle.com, which contained datapoints for each attempted shot in each game that season, along with properties of that shot, such as distance, success of shot, closest defender, time on shot clock, and time of game. This dataset had 21 columns and 128,069 rows.

## Analysis ##
Bear Analysis

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

Naveen Analysis

*Question 1:* What were the shot results from various distances?
*Figure 1:* 
![image](https://github.com/bearstmichael/proj1-group-3/assets/128173190/f7dc3547-1f6f-4419-9994-c28a98345821)
![image](https://github.com/bearstmichael/proj1-group-3/assets/128173190/4ddc08f1-9836-4234-8c3d-ca092dee4af8)
![image](https://github.com/bearstmichael/proj1-group-3/assets/128173190/2d280a76-ed1a-4cbf-8542-7f975190be47)

The first pie chart addresses every shot taken in the data set from all distances. Slightly more shots were missed (54.4%) than made (45.6%). The second pie chart shows the shot results for all distances less than 5 ft. At a distance of 5 ft more shots were made (61.9%) than missed (38.1%). This could be explained by the fact that this distance range covers layups which are shots that are rarely missed at this level of play. The final pie chart shows the shot results for all distances greater than 35 ft. At this distance, more shots are missed (78.6%) than made (21.4%).

*Figure 2:*
![image](https://github.com/bearstmichael/proj1-group-3/assets/128173190/530943db-0415-498f-9081-b1538b9e957d)

This bar chart is a representation of the number of made shots according to binned distance values. It is important to note that this chart represents the total number of made shots and does not account for the differential amount of shots taken at each distance. For example, more shots are likely to be taken outside of the 3 point mark for increased value. This would explain the increased height of the bin (marked with blue line) that includes the distance 3 pointers are shot from. There is another peak at distance <5 ft so we can conclude that most shots that are made are in the range of less than 5 ft from the net and between 20 - 24.9 ft from the net.

*Figure 3:*
![image](https://github.com/bearstmichael/proj1-group-3/assets/128173190/92e7483d-4b45-48ef-9171-8d1e237fd3a1)

This line graph shows the relationship between percent of shots made and distance. This accounts for the number of shots taken so we can get a more clear picture of what happens with the shot result as the distance increases. This graph shows a clear relationship between shot result and distance which is that as the distance increases, the percent of shots made decreases. In other words, the farther from the net you shoot, the more likely you are to miss.

*Question 2:* When are shots made on the shot clock and how does that affect shot result?
*Figure 4:*
![image](https://github.com/bearstmichael/proj1-group-3/assets/128173190/b96b5ad6-e2ee-41c5-8abe-5cde29d3f90c)

This bar chart is a representation of the number of made shots according to binned shot clock values. The shot clock is a clock that starts upon a player receiving the ball and counts up to 24 seconds at which point the player must either shoot or pass the ball. This figure shows that most shots are made between 8 to 16 seconds on the shot clock. Similarly to figure 2, however, this figure does not account for the differential amount of shots taken for each binned shot clock value. It could be that more shots are taken during the 8 to 16 second time period.

*Figure 5:*
![image](https://github.com/bearstmichael/proj1-group-3/assets/128173190/62b071ed-0b17-4b31-82bf-d874b4b08252)

This line graph shows the relationship between percent of shots made and shot clock time. This accounts for the number of shots taken over the course of the shot clock so we can get a better picture of the relationship between shots made and shot clock time. This figure illustrates a clear positive relationship between these two variables such that as the shot clock time increases, the percentage of shots made increases as well. This makes sense because as players have a longer time to shoot the ball they are better able to do so.

