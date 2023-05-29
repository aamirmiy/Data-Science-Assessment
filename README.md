# Data-Science-Assessment
Findings:
1. Clearly we can see in the higher league index we have more younger players which is kindoff understandable as young players tend to have higher stamina, reflexes and muscle memory for gaming as compared to the senior level players. 
2. Highly league player tends to spend more time playing.
3. Removing ActionsinPAC and UniqueUnitsMade as we can see in the heatmap above this feature is weakly correlated with our target but has high VIF. Also we can remove SelectByHotkeys as this is highly correlated with AssignToHotkeys where AssignToHotkeys is better correlated with our target.
4. We clearly see that NumberOfPACs is highly correlated to Action Latency. Also GapBetweenPACs is highly correlated with NumberOfPACs. Also TotalMapExplored is highly correlated with Action Latency and ComplexUnitsMade. Hence we remove NumberofPACs, GapBetweenPACs , TotalMapExplored. 
5. From the above correlation heatmap we can draw some hypothesis:
Action latency significantly seems to have significant negetive correlation with our target variable. This is kind of very obvious that lower the action latency a player has, the better the player is and better the chances to be playing in higer leagues.
Total hours/ hours per week seems to have decent correlation value with our target. The hypothesis here is that more practise a player does, the better he performs in the leagues and has more chances to be in the higher leagues. Although its alone not significant.
AssignToHotKeys have a correlation value of 0.53 with the target. This implies that player having higher number of units or buildings assigned to hotkeys per timestamp have better chances to play in the higer leagues.
Minimapattacks, WorkersMade also have high correlation hence can be an important predictor for our target


For future data collection:
1. Store age in terms of age groups.
2. Number of matches played.
3. Number of matches won.
4. Number of matches lost. 
These additional features would help in making more informed decisions.
