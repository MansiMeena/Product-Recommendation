# Product-Recommendation
Kaggle Competition : Santander Product Recommendation

(https://www.kaggle.com/c/santander-product-recommendation)

Santander Bank offers a lending hand to their customers through personalized product recommendations. In their second competition, Santander is challenging Kagglers to predict which products their existing customers will use in the next month based on their past behavior and that of similar customers.

Competition data consists of customer data from 2015-01 ~ 2016-05 (total of 17 month timestamps) including customer's demographic information and their product purchase behavior. Competition challenges you to predict top 7 products out of 24, that each customer in the test data is most likely to purchase on 2016-06.

Evaluation metric is in MAP@7, which made the direct optimization difficult during training phase. Instead, the mlogloss was widely used among kagglers to indirectly optimize the solution.

With BreakfastPirates generous sharing, using 2015-06 data-only as a training data seemed to perform pretty well in the leaderboard (reaching almost ~0.03). Single model performance was enough to place you on top of the leaderboard, since MAP@7 made the effect of ensemble relatively weak.

As always, feature engineering seemed to be the most important factor in this competition, along with good cv scheme to reach the best hyper-parameter that squeezes the performance from the given data.
