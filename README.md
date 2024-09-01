# NBA Data Exploration

## Overview
This project involves analyzing NBA data to explore possible associations between teams, win rates, playoff appearances, and more. 
The dataset is sourced from FiveThirtyEight's analysis (http://fivethirtyeight.com/interactives/the-complete-history-of-every-nba-team) and contains both original data from (http://www.basketball-reference.com/).


## Data Description
The dataset has been split into two subsets:
1. **nba_2010**: Games from the 2010 season.
2. **nba_2014**: Games from the 2014 season.


### Key Columns:
* `fran_id`: Franchise identifier (team name)
* `pts`: Points scored by the team
* `opp_pts`: Points scored by the opponent
* `point_diff`: Difference between `pts` and `opp_pts`
* `forecast`: Predicted probability of winning the game
* `game_location`: Location of the game (home/away)
* `game_result`: Result of the game (win/loss)


## Objectives and Analysis Tasks
### Descriptive Statistics
1. **Compare Points Scored by Teams (Knicks vs. Nets)**:
   - **Task**: Using the `nba_2010` data, create two series (`knicks_pts` and `nets_pts`) representing points scored by the Knicks and Nets, respectively.
   - **Analysis**: Calculate the difference in average points scored between the Knicks and Nets for the 2010 season and determine if the points scored (`pts`) are associated with the teams (`fran_id`).

2. **Distribution Analysis of Points Scored**:
   - **Task**: Create overlapping histograms for `knicks_pts` and `nets_pts` to visualize the full distribution of points scored and assess if the mean difference is meaningful.
   - **Analysis**: Compare the distributions and determine if they appear to be the same.

### Comparative Analysis
3. **Compare 2010 vs. 2014 Seasons**:
   - **Task**: Replicate the analysis steps from the 2010 data using `nba_2014`. Calculate the difference in average points scored by the Knicks and Nets in 2014 and create overlapping histograms.
   - **Analysis**: Evaluate if the difference in points scored between the teams increased or decreased from 2010 to 2014 and if the calculated mean differences align with the histogram visualization.

### Inferential Statistics
4. **Team Performance Analysis Using Boxplots**:
   - **Task**: Generate side-by-side boxplots for points scored (`pts`) by different teams using the `nba_2010` data.
   - **Analysis**: Determine if there is any overlap between the boxplots, suggesting an association between team (`fran_id`) and points scored (`pts`). Identify which teams, if any, have significantly different average scores per game.

5. **Game Outcome Analysis Using Contingency Tables**:
   - **Task**: Create a cross-tabulation (contingency table) to analyze the frequency and proportion of wins and losses for the 2010 season.
   - **Analysis**: Determine if game location (`game_location`) and game result (`game_result`) are associated using an `expected contingency table and Chi-square` statistics.

### Correlation and Covariance Analysis
6. **Correlation Between Game Predictions and Actual Outcomes**:
   - **Task**: Calculate the covariance between `forecast` (predicted probability of winning) and `point_diff` (points scored difference).
   - **Analysis**: Assess if teams with a higher predicted probability of winning tend to win by more points.

7. **Correlation Coefficient Analysis**:
   - **Task**: Calculate the correlation between `forecast` and `point_diff` to determine if a statistical association exists between the prediction and the point difference.
   - **Analysis**: Evaluate the strength and direction of the correlation.

### Visualization
8. **Scatter Plot Analysis of Predictions vs. Points Difference**:
   - **Task**: Create a scatter plot of `forecast` (x-axis) and `point_diff` (y-axis) to visualize the relationship.
   - **Analysis**: Determine if the scatter plot supports the calculated correlation value.


## Conclusion
This project employs various `statistical techniques` to analyze and visualize NBA data, including:
`descriptive statistics`, 
`inferential statistics (Chi-square test)`, and 
`correlation analysis`. 

Through this exploration, we aim to uncover patterns and associations in NBA game results, team performances, and predictive modeling.


## Installation and Usage

To run the analyses and create visualizations, ensure you have the following Python packages installed:
- `pandas`
- `matplotlib`
- `seaborn`
- `scipy`


## Acknowledgments
The dataset used in this project was sourced from FiveThirtyEight's analysis and Basketball Reference.


## Contributing
Feel free to fork the repository, create a pull request, or report issues. Contributions are welcome!



