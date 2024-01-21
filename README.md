# Statistical Analysis, Hypothesis A/B Testing
As a data professional in a data consulting firm, called Automatidata. The current project for our newest client, the New York City Taxi & Limousine Commission.

## Project objectives
Using A/B Testing to analyze the relationship between fare amount and payment type.

In this project, I will practice using statistics to analyze and interpret data. The activity covers fundamental concepts such as descriptive statistics and hypothesis testing. I will be exploring the data provided and conduct A/B and hypothesis testing.  
<br/>  

### The purpose ## 
This project is to demostrate knowledge of how to prepare, create, and analyze A/B tests. My A/B test results aim to find ways to generate more revenue for taxi cab drivers.

**Note:** For the purpose of this project, assume that the sample data comes from an experiment in which customers are randomly selected and divided into two groups: 1) customers who are required to pay with credit card, 2) customers who are required to pay with cash.

### The Goal ###
To apply descriptive statistics and hypothesis testing in Python. The goal for this A/B test is to sample data and analyze whether there is a relationship between payment type and fare amount. For example: discover if customers who use credit cards pay higher fare amounts than customers who use cash.
  
### This projects has four parts: ###

**Part 1:** Imports and data loading
* Includes loading packages necessary for hypothesis testing.

**Part 2:** Conduct EDA and hypothesis testing
* Compute descriptive statistics to help in data analyze.

* Forumlate null hypothesis and alternative hypothesis.

**Part 3:** Communicate insights with stakeholders

* What key business insight(s) emerged from the A/B test.

* What are the proposed business recommendations based on the results.

Shows how many payments are there for each payment type
![image](https://github.com/Lawrence-le/statistical-analysis-AB-Testing/assets/151991077/3bf56947-fa7e-48e9-9fb7-0b6c7d8a49f0)

Shows the mean amount for each payment type
![image](https://github.com/Lawrence-le/statistical-analysis-AB-Testing/assets/151991077/e37a43ce-9fb8-450c-a87a-48d375300d7e)

### Hypothesis testing

**Null hypothesis**: There is no difference in average fare between customers who use credit cards and customers who use cash.  
**Alternative hypothesis**: There is a difference in average fare between customers who use credit cards and customers who use cash

**Objective:** To conduct a two-sample t-test.  

Steps for conducting a hypothesis test: 

1.   State the null hypothesis and the alternative hypothesis
2.   Choose a signficance level
3.   Find the p-value
4.   Reject or fail to reject the null hypothesis 

**The Hypothesises**  

H0: There is `no difference` in the average fare amount between customers who use credit cards and customers who use cash.  
H1: There is `a difference` in the average fare amount between customers who use credit cards and customers who use cash.  

Choose `5% as the significance level` and proceed with a two-sample t-test.

t-statistic: 6.87%  
P-value: 0.0000000007%

There are two main rules for drawing a conclusion about a hypothesis test:   
•	If `p-value` < `significance level`, **reject** the null hypothesis.  
•	If `p-value` > `significance level`, **fail to reject** the null hypothesis.    

In this scenario, the p-value of 0.0000000007% is < significance level of 5%  
So we **reject** the null hypothesis

We can conclude based on the hypothesis testing that there is a `statistically significant difference` in the average fare amount between customers who use credit cards and customers who use cash.

### What are the proposed business recommendations based on the results

1.   The key business insight is that encouraging customers to pay with credit cards can generate more revenue for taxi cab drivers. 

2.   This project requires an assumption that passengers were forced to pay one way or the other, and that once informed of this requirement, they always complied with it. The data was not collected this way; so, an assumption had to be made to randomly group data entries to perform an A/B test. This dataset does not account for other likely explanations. For example, riders might not carry lots of cash, so it's easier to pay for longer/farther trips with a credit card. In other words, it's far more likely that fare amount determines payment type, rather than vice versa. 


