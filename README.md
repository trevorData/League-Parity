# [Main Plot](https://imgur.com/EpQH2vW.jpg)

---
### Summary:

**TLDR:**

League | When is the Season 90% "solved"?
---|---
NBA | 48 games (57% of season)
MLB | 111 games (68% of season)
NHL | 63 games (76% of season)
NFL | 13 games (76% of season)

---

League | How much of next year's record can be predicted from this year's record?
---|---
NBA | 40%
MLB | 26% 
NHL | 19%
NFL | 12%

---

### **How R\^2 works:**

R^2 is a measure of how well we can predict a dependent variable using an independent variable. It ranges from 0 to 1 and tells us "out of all the variation in the dependent variable, what % can be predicted using the independent variable?".

In this case, if we look at team records midway through a season, the R^2 tells us how much of the variation in the end-of-season records can be accounted for using that mid-season record.

Naturally, the R^2 will be low at the start of each season because we have little information to work with; good teams have not yet had a chance to separate themselves from the bad teams. As the season progresses, we get a better idea of just how good each team really is, and R^2 starts to increase. At the end of the season, when every team's record has been decided, we can perfectly predict team records so R^2 will equal 1.

---

### **How the leagues differ:**

The thin horizontal line represent an R^2 of .9, to indicate when 90% of the variation in end-of-season records can be predicted. 

We see that the NBA crosses this line very early, when only 57% of the season has been completed, or after about 48 games. In contrast, the MLB crosses this line after 68% of the season (111 games) and the NFL and NHL both cross after about 76% of the season (13 games and 63 games, respectively).

This difference is to be expected, as the NBA has a high amount of scoring opportunities and long season that serve to reduce the effect of randomness, while the NFL is much more at the mercy of chance.

This leads me to believe that the NBA could stand to shorten their season dramatically while seeing a negligible change in end-of-season standings. Hopefully this would lead to less player injuries and solve the ["load management"](https://www.espn.com/nba/story/_/id/28066201/nba-load-management-know-know) issue that has been plaguing the league the past few seasons.

---

### **What about parity between seasons?**

Between players aging, free agency moves, and the rookie draft, each league will have a "regression to the mean" across seasons, with dynasties eventually crumbling and bad teams eventually putting the pieces together. The strength of this effect varies by league and seems to generally fall along the same lines as in-season parity, with the NBA having the most inertia and the NFL being the most susceptible to chance.

### [NFL](https://imgur.com/WhyiIyX.jpg)
### [NHL](https://imgur.com/n786rDs.jpg)
### [MLB](https://imgur.com/h848GH5.jpg)
### [NBA](https://imgur.com/hMYdsCu.jpg)

### **What causes this?**

Because the NBA has smaller rosters and fewer players on the court, good teams tend to stay good as long as their best players stick around and stay healthy. In contrast, careers in the NFL are short, large rosters see a lot more shuffling, and injuries to key players can derail a team's season instantly. 

40% of the variance in NBA records can be predicted using the records from the previous season, while for MLB, NHL and NFL it is only 26%, 19% and 12% respectively.

This makes the Patriot's multi-decade run look even more impressive!

---

### [Bonus Plot](https://i.imgur.com/jCnwsj8.png)

I was curious what it would look like if I created a league that had no parity at all, so I simulated 10 seasons for an imaginary league where higher seeds defeat lower seeds every time.

This imaginary league has 30 teams, and a 29 game season where each team plays the others exactly once. Because wins are pre-determined by seeding, the only randomness is in the scheduling each season.

---

### **Sources:**

NFL, NBA and MLB data taken from 538.  
NHL data taken from Kaggle

**Data used was for past 10 seasons, except for NHL where it was for past 9.**  
Teams that had their season shortened due to cancellations or lockouts were thrown out. In the case of MLB, if a season had extra games I capped it at 162.
