# worlds_group_draw

I thought I should simulate the group draw, unordered and ordered to reach the following results : 

- individual group probability
  
- individual matchup probability
  
- who has the best chance at getting an easy group

# Method

I chose the big 3 + UOL out of playins

- A group is valid if there are no 2 teams from the same region
  
- First determine all valid draws
  
- Then draw in order, and to know if we can place the team in a group find out if there is a valid draw we can obtain from this position.

The last point is the most important part : we can’t just look at regions and add teams if they can fit in. We need to consider all future draws to see if we can reach a valid state. For an example of this, I repost this timeless classic of TSM Loco and Reginald making this mistake in 2015 
https://youtu.be/6JRWRYeGomc 

# Results

My main takeaways : 
- 333116 (4! ** 4) possible draw orders, 1440 unique results, 40 unique groups
- Most likely group : TSM DRX ROG LGD (24% of scenarios), but TSM vs ROG only has a 33% of happening
- TSM is 1.4 more likely to face FNC than other pool2 matchups
- G2 vs a China pool2 team (JDG/SNG) has a 77% of happening (I’m sweating), rather than the intuitive 66%
- MAD vs FLY at 47% for the spicy botlane Ignar vs Kaiser matchup
- DRX are the lucky winner and get to face the world champs early (57%)
