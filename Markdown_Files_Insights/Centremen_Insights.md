
# Centremen Data Analysis
In this section, I analyze the points attained by players who strictly play the centre ('C') position. The analysis in this section only applys to centrement who DO NOT play a secondary position (excludes players who play C/RW, C/LW OR C/LW/RW). 

### Centremen Point Totals by Week

![Centremen Points by Week](https://github.com/carsonbennett1/Hockey-Player-Analysis-Project/blob/main/img/centremen_point_by_week.png)

### Centremen Point Summary as of Week 13

![Centremen Point Sum](https://github.com/carsonbennett1/Hockey-Player-Analysis-Project/blob/main/img/centremen_point_summary.png)

### Centre Boxplot Insights
Below is the centre boxplot for centremen (and only centremen exclusively) that display their median weekly points, and their quartile range throughout the first 13 weeks. More on the findings of this image below...

![box](https://github.com/carsonbennett1/Hockey-Player-Analysis-Project/blob/main/img/centre_boxplot.png)

After looking at the graph above, it is apparent that the median weekly points for Hischier, Point, and Schiefele is considerably low for players who have a season rank of 20, 18, and 26 respectively. They are amongst the 30 best NHL players amongst fantasy points, and keep up amongst the best in NHL stats (as of January 14th, 2025) to back it up as well:
- M.Schiefele: T-9 in league points, T-3 in league goals (26), 26 assists
- B.Point: T-5 in league goals (25), 22 assists, 47 points
- N.Hischier: 20 goals, 17 assists, +14
However, these players have also been injured for a number of weeks. This is important because of the way I collected CSV stats. If a player was injured, I recorded that weeks stats as 0, and not NaN. This means that the boxplot above accounts for weeks where they put up zero points, and for player like B.Point who missed 4 weeks (thus 4 zeroes), this can have a significant affect on the findings.

To account for this, weeks where players were injured now have NaN in their place instead of 0. This way we can look at the true efficiency of the players when they are healthy. The boxplot below is a more fair representation of player performance.

![box_two](https://github.com/carsonbennett1/Hockey-Player-Analysis-Project/blob/main/img/centre_boxplot_nan_excluded.png)