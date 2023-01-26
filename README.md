
## Background
Second Harvest Heartland is a nonprofit organization working towards ending hunger through community partnerships. 
They procures food from different sources, partner with community services like food shelves and meal programs, and as provided 105 million meals in 2021 alone.

## Task
Using 2 years of data to understand factors affecting donation outcomes based on earned media for Second harvest heartland and build a machine learning model to predict donation amount.

## Action
#### "data processing and linear model.ipynb"
  1. Categorized earned media into 4 categories.
  2. Ran linear model on donation amount and calculated variation by changing window values (highest explained variation is best to do the roll-up).
  3. Apply different rolling effect on different media channel.
  4. Break into 2  scenarios (holiday and non-holiday) for 2 different client types (individual and organizaiton), and implement separate models. (cause data in those situations are really different)
  5. Build linear exploratory model to see the coefficents of each features, and draw relationship between features and the frequency of donation.

#### "models.rmd"
  6. Build random forest predictive model focusing on donation amount in order to predict the most valuable earned media.(in )


## Result
#### In holiday 
  Web article has the largest donation amount for both organization and individaul, and tv is the worst for both client types.
#### In non-holiday 
  For organizationm, web article still has the largest donation amount and tv is the worst. But for individual, web article is the worst and tv the largest donation amount.

## Finding
  1. Organizations were barely influenced by earned media and campaigns since we could explain less than 3% of the variation using our model. 
  2. TV was by far the best when it comes to non-holiday months. It drives about 12 times the number of donations and amounts for non-holiday months compared to the next highest source.
  3. For campaign data, SHH events and acquisition mail were the most important, and e-appeals were good at driving a high donation amount.
