# Analysis

## ANOVA - Finding significant features

One-way ANOVA on the 10 given features showed that the significant predictors of house pricing were Overall Quality, Exterior Quality, Kitchen Quality, Basement Quality (height), Central Air Conditioning, Lot Shape and Fireplace Quality. Land Slope, Month Sold and Year Sold were not significant at the 5% level.

We then ran two-way ANOVA on pairs of significant features using a full-factorial model to test interaction effects. The majority of feature pairs (19 out of 20) showed statistically significant interaction terms with the house price. However, inspection of contingency tables revealed that some factor combinations were sparse or missing, indicating that the factorial design is unbalanced. As a result, some interaction effects may be influenced by limited or uneven data coverage across category combinations.

Since the dataset is observational rather than experimental, the features are not independently assigned.
Instead, features such as Overall Quality, Exterior Quality and Kitchen Quality show strong associations, reflecting underlying relationships in housing characteristics rather than independent experimental factors. Therefore, the observed interaction effects should be interpreted as statistical associations within the dataset rather than controlled interaction effects.

We applied Tukey's HSD test to the significant features found in the one-way ANOVA analysis. The results show a strong ordered relationship between quality features (including the presence of central air conditioning) and house price, with significant differences between high and low categories, while adjacent categories occasionally overlap.

For lot shape, the results show mixed patterns between categories. Significant effects are found between IR1 and IR2, as well as between both IR1 and IR2 as compared to the regular (Reg) lot shape. However, IR3 does not show statistically significant differences from any other category, suggesting it is not clearly distinguishable in terms of price from other lot shapes in this dataset. Overall, the results do not indicate a consistent pattern in price differences across the groups.