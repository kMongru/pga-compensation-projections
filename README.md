# pga-compensation-projections

### Objective:

This analysis will determine the how of different performace indictors (based on domain knowledge) in PGA tour events effect scoring. These indicators include:

- driving distance
- driving accurary
- greens in regulation
- scrambling
- sand saves
- putts per round

My hypothesis:

- The idiom "drive for show putt for dough" is true in respect to scores
- That greens in regulation is the strongest indecator affecting performance

### Overview:

The data collected in this analysis was scraped with the python's requests and panadas library from https://www.pgatour.com/stats and aheres to the site's web scraping clause (robot.txt). The data was cleaned and visualized with matplotlib to understand the nature of the data and choose an appropriate model. This data set was then divided following the 80/20 rule to create a training and testing set. The data analysis then performed using a linear regression learning model. The model were then optimized by normalizing features based on z-score and adjusting the base value.

### Conclusion:

The model was able to predict scores with 1.3 strokes. The correlation analysis showed that driving distance is positively correlated with strokes gained and has a larger impact than putts. The most influencial factor is proximity to the hole (0.3465).

![results](https://github.com/kMongru/pga-performance-analysis/blob/main/results.png)
