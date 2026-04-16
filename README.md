# MSBA-Capstone-Project

## Business Problem & Project Objective
MasterControl’s Manufacturing Solutions product (Mx) is significantly underperforming compared to its Quality Solutions product (Qx). The company believes it may not be targeting the right companies or the right people within those companies, leading to missed revenue opportunities and wasted marketing expenditures.

We have been given 16,644 qualified sales leads (QALs) from Jan 2024 to Dec 2025. These come from 15,371 unique contacts across 14 different variables. The goal of this project is to identify which account and contact characteristics are the most predictive of lead progression.

## Solution
Before creating our models, we cleaned and prepared the data by handling missing values, defining and creating the target variable, and feature engineering.
We then found the baseline conversion rates for Mx, Qx, and the various variables that we analyzed (industry, manufacturing model, site function, etc).

Because this is a binary classification problem (will leads convert? Yes or No?), we created and comapred a few models: Logistic Regression, Random Forest, Gradient Boosted, and Decision Tree.

Through these models, we identified a few statistically significant indicators of conversion on both the account level and contact level that we synthesized into recommendations for MasterControl to take action on.

### Mx Target Account
**Target / Prioritize**
Manufacturing Model: CMO, CDMO.
Account Tier: Small, Medium.
Site Function: Any actual manufacturing site.
Industry: Blood & Biologics, Medical Device, Pharma & BioTech.

**Avoid**
Manufacturing Model: -
Account Tier: Large.
Site Function: Non-manufacturing.
Industry: Non-Life Science.

### Mx Ideal Contact
**Target / Prioritize**
Title: VP / Heads.
Channel: Direct / Inbound, SEO.
Priority Signals: Contact Us, Live Demo, Video Demo.

**Avoid**
Title: Unknown.
Channel: External Demand Generation, Email, Events, Outbound.
Priority Signals: Webinar Demo, P2.

## Business Value of Solution
Through our analysis, we found that the Mx and Qx products are fundamentally different in their target markets and should prioritize different leads. While there are cross sell opportunities, we found that by focusing on the above mentioned account and contact profiles, the baseline conversion rate for Mx (which is at 13%) can be significantly increased.

For example, when we focus specifically on CMO and CDMO accounts, the conversion rate jumps to 17%. Targeting leads where demos or speaking to someone in the company requested, that jumps to 28%. This requires no additional spending or new hires, simply calling the right people.

Because the gap between Mx and Qx conversion rates is not a product issue but a targeting issue, if MasterControl focuses their resources on pursuing the highest converting leads, they can significantly improve their conversion rates.

## Individual Contribution 
To complete this project, each group member individually completed the exploratory data analysis and modelling. After completing each step, we met as a group and compiled clean, unified code based on the strengths of each of our codes.

I was responsible for creating the slides that summarized our statistically significant findings for Mx target accounts and Mx target contacts. I was also in charge of the slide that went over the cross tabulation between site function and title.

## Difficulties Encountered
I would say that one of the main difficulties we encountered was the lack of data for certain leads. We could not find statistically significant results for certain variables because there were not many records that we could analyze. So, while we could find interesting statistics, we could not confidently say they were reliable.

I think it was also quite difficult to take our model findings and translate them into plain English. Presenting technical information to non-technical audiences was an interesting challenge. I went about solving this by convering coefficients into odds that could easily be explained (ex: CMO had 1.7x the odds of converting compared to CDMO).

## What I Learned
I learned that defining the business problem clearly and understading exactly what we are looking to find before doing anything else is the most important step in data analysis. I could easily see a scenario where we overcomplicated the analysis and models because we didn't clearly understand that we were looking at a binary classification problem and we were looking for strong conversion indicators.

Additionally, the process of EDA is extremely important and allowed easy and smooth model creation. If any of our data cleaning or feature engineering was off, our models would not be accurate.
