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

- the idom "drive for show putt for dough" is true in respect to scores
- that greens in regulation is the strongest indecator affecting performance

### Overview:

The data collected in this analysis was scraped with the python's requests and panadas library from https://www.pgatour.com/stats and aheres to the site's web scraping clause (robot.txt). The data analysis was performed using a linear regression to discover statisically significant values and create a IIP data set. This data set was divided creating 80/20 training and testing sets. The training set was used with random forest, XXX, and XXX models to discover systematic relationships. The models were then optimized by normalizing features based on z-score and adjusting the base value.

### Conclusion:

The model was able to predict scores with 1.6 strokes. The correlation analysis confirmed that

![results](https://github.com/kmongru78/pga-performance-analysis/results.png)
