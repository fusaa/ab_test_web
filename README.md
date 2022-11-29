## Website product page conversion rate A/B test
  
In this notebook we are going over the approach of executing a simple A/B using data available from [Kaggle](https://www.kaggle.com/datasets/zhangluyuan/ab-testing). To make things more enjoyable let´s create a hypothetical circumstance to illustrate the problem better. You can  click here now to jump right into the  [Jupyter Notebook](https://github.com/fusaa/ab_test_website_conversion/blob/main/notebook.ipynb).

"Electronic Masters" is an online store for computer products. Consumers can buy devices like monitors, computers, laptops, HDMI cables, home theatre systems, batteries, headphones, etc. The UX design team has been working on a new sales page to increase conversion rates for a distinctive type of battery that costs £4.99.  

The current conversion rate of the product webpage is at 13% on average over the last year. The intent of the product manager is to boost the conversion rate by 2%. The new page, developed by the UX team, would be a success if the conversion rate evolved to 15%. Before replacing the old sales page with the new one, it is wise to try its effectiveness on a smaller group of customers, running a smaller risk of losses if the new page shows a conversion worse than the current page. The dev team has implemented the online test with the new page and provided the dataset for examination.

## The experiment

We will choose a two-tailed test. The new page can perform both ways, better or worse.

H0: New page conversion is the same. - The null hypothesis.  
H1: New page conversion is different. - The alternative hypothesis.

Let´s keep the confidence level at 95%, bringing this way a significance level of 5%. That means we can be 95% confident the samples include the true population mean. On the other hand, the significance level is the probability of wrongly rejecting the null hypothesis. In this case, we run a 5% chance of rejecting the null hypothesis when in fact, we should not.

At a later stage, the significance level will be compared with a calculated metric(p-value) using statistical methods. If the p-value is less than the significance level, it means we can reject the null hypothesis and conclude that the effect is statistically significant with a 95% confidence level.



# The test
| Group      | Converted   | Total   |
|    :----:  |    :----:   |  :----: |
| control    | 560         | 4720    |
| treatment  | 565         | 4720    |


Chi Squared Test was used in the test, check the results [here](https://github.com/fusaa/ab_test_website_conversion/blob/main/notebook.ipynb).



