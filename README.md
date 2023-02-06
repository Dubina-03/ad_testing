# ad_testing

This time I decided to practice my knowledge that I gained by taking several courses, so I analyzed and interpreted the results of ***A/B testing*** with ***hypothesis tests*** and ***Confidence Interval***.

Steps:

1. Source of data: [Kaggle](https://www.kaggle.com/datasets/osuolaleemmanuel/ad-ab-testing).
2. Data Manipulation. The data has been preprocessed with
3. ***Hypothesis*** :
    - H0: there is no difference between conversion success of new and old advertisment  
    - Ha: there is difference between conversion success of new and old advertisment  
    I decided to do a ***z-test*** sinse the values are independent, we have 2 groups and sample sizes are large.
4. 95% ***Confidence Interval***
5. Looking at different features (in case of big difference conduct a hypothesis test)
### Results
The p_value = 0.51849 that is much larger than our significance level = 0.05, so ***we can't reject the null hypothesis***. It means that there is no significant difference between proportion of conversions new and old ad.  
And also our ***confidence interval (-0.07377294, 0.0372017)*** which gives us the same result as the hypothesis test because the value 0 is inside the interval   
 For other characteristics, there was ***no significant difference*** between the values.

***Techniques***: hypothesis tests (z-test), Confidence Interval  
***Libraries***: pandas, numpy, matplolib.pyplot, seaborn, statsmodels.stats.proportion.
