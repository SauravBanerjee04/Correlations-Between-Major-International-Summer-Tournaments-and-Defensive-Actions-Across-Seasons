# Correlations-Between-Major-International-Summer-Tournaments-and-Defensive-Actions-Across-Seasons: Analyzing the Effect of Fixture Congestion on Premier League Players

## Authors
Saurav Banerjee and Joshua Park

## Overview
This project investigates the impact of fixture congestion on player fatigue in the Premier League, particularly focusing on defensive statistics. It examines whether participation in major international tournaments like the World Cup affects players' performances in the following seasons, due to inadequate rest and recovery time.

## Problem Statement
In recent years, both coaches and players have expressed concerns about the increased number of matches and insufficient rest periods. This project aims to explore how playing in the World Cup, which eliminates the summer break, impacts player fatigue, with a particular focus on defensive actions.

## Literature Review
1. **Injury Statistics**: During the 2014 World Cup, 104 injuries were reported, with an injury rate of 1.68 per match (Junge & Dvorak, 2015).
2. **Performance and Injury**: Lower injury burden and higher match availability are linked to better league rankings and success in European competitions (Hagglund et al., 2013).
3. **Fatigue and Recovery**: Sprint performance and muscle soreness worsen after 90-minute games, with full recovery taking at least 48 hours (Rampinini et al., 2011).
4. **Mental Fatigue**: This has a negative effect on tactical performance, especially in defensive actions (Kunrath et al., 2020).

## Data Collection
The data was collected from FBREF’s datasets, focusing on the Premier League. The datasets were exported as CSV files for the 2017-18, 2018-19, and 2019-20 seasons, then processed and analyzed using Python libraries Pandas and SciPy.

## Focus on Defensive Actions
Due to the lack of datasets on distance traveled, the project focuses on defensive actions, which reflect how much effort players exert off the ball. Mental fatigue in soccer often leads to reduced tactical and cognitive performance, particularly in defense.

## Metrics Analyzed
- **Pressures in the Attacking Third**: High pressing requires significant energy, making it a key indicator of fatigue.
- **Errors**: Mental fatigue can lead to an increase in errors.

## Hypotheses
1. **Pressures in the Attacking Third**:
   - Null Hypothesis (H0): Means of pressures in the attacking third are equal across the 2017-18, 2018-19, and 2019-20 seasons.
   - Alternative Hypothesis (HA): Means of pressures in the attacking third during these seasons are not equal.

2. **Errors**:
   - Null Hypothesis (H0): Means of errors are equal across the 2017-18, 2018-19, and 2019-20 seasons.
   - Alternative Hypothesis (HA): Means of errors during these seasons are not equal.

## ANOVA Analysis
- **Conditions**:
  - **Random**: Random selection of seasons, with 2018-19 chosen by a coin flip to compare with adjacent seasons.
  - **Normality**: Not all distributions were perfectly normal, but most were approximately normal.
  - **Equal Variance**: Residual plots showed roughly equal scattering.

## Results
The ANOVA analysis did not reveal statistically significant differences between the seasons following World Cup years and regular seasons. However, the trends discussed in previous literature might be obscured by confounding variables.

## Drawbacks and Confounding Variables
- **Link Between Pressures and Fatigue**: There is an uncertain link between pressures in the final third and fatigue, as players may push through pain.
- **Team Impact**: Different teams have varying numbers of players participating in the World Cup, affecting their results differently.

## Conclusion
While the study did not find significant statistical evidence of fatigue affecting defensive actions post-World Cup, further research is needed to account for various confounding factors. Future studies could focus on more precise metrics of player fatigue and explore additional variables that might affect player performance.

## File Summaries

### Data Files
- **1718processed.csv**: Contains processed data for the 2017-18 Premier League season, including various defensive statistics for each team.
- **1819processed.csv**: Contains processed data for the 2018-19 Premier League season, similar to the 1718 file, with updates for that season's performance.
- **1920processed.csv**: Contains processed data for the 2019-20 Premier League season, with the same format as previous seasons, focusing on defensive actions.

### Code and Analysis
- **finalproject.ipynb**: A Jupyter Notebook containing the complete analysis, including data loading, preprocessing, and statistical testing using ANOVA. It uses Python libraries such as Pandas, NumPy, Matplotlib, and SciPy to analyze the data.
- **finalproject.html**: An HTML export of the Jupyter Notebook, allowing for easy viewing of the analysis and results without needing a Jupyter environment.

### Documents and Presentation
- **finalproject.pdf**: A detailed report summarizing the project's objectives, methodology, results, and conclusions. It includes tables and figures from the analysis and discusses the implications of the findings.
- **RS3 Final Project Presentation.pptx**: A PowerPoint presentation outlining the project, including the problem statement, hypotheses, methodology, results, and key takeaways. It is designed for presenting the project findings to an audience.

## References
1. Hägglund M., et al. (2013). Injuries affect team performance negatively in professional football: An 11-year follow-up of the UEFA Champions League Injury Study. British Journal of Sports Medicine.
2. Junge A., & Dvořák J. (2015). Football injuries during the 2014 FIFA World Cup. British Journal of Sports Medicine.
3. Kunrath C. A., et al. (2020). Mental fatigue in soccer: A systematic review. Revista Brasileira de Medicina do Esporte.
4. Rampinini E., et al. (2011). Match-related fatigue in soccer players. Medicine and science in sports and exercise.
