# Foodie_fi_SQL_Case_Study_Solution
This repository contains my solution to Week 3 Danny Ma's 8-week SQL challenge on Subscription base business analyses

#### Introduction
Subscription-based businesses are super popular and Danny realised that there was a significant gap in the market. Danny created Foodie-Fi with a data-driven mindset and wanted to ensure all future investment decisions and new features were decided using data. This case study uses subscription-style digital data to answer critical business questions.

#### Available data
Danny has shared the data design for Foodie-Fi and also short descriptions on each of the database tables - our case study focuses on only 2 tables but there will be a challenge to create a new table for the Foodie-Fi team.

#### Entity Relationship Diagram
![image](https://github.com/DataStance1/Foodie_fi_SQL_Case_Study_Solution/assets/114801619/bebee734-c09e-480b-9fa6-46fce5f2dc2f)

#### Table1: Plans
- Customers can choose which plans to join Foodie-Fi when they first sign up.
- Basic plan customers have limited access and can only stream their videos and is only available monthly at $9.90
- Pro plan customers have no watch time limits and are able to download videos for offline viewing. Pro plans start at 19.90 a month or 199 for an annual subscription.
- Customers can sign up for an initial 7-day free trial and will automatically continue with the pro monthly subscription plan unless they cancel, downgrade to basic or upgrade to an annual pro plan at any point during the trial.
- When customers cancel their Foodie-Fi service - they will have a churn plan record with a null price but their plan will continue until the end of the billing period.

#### Table 2: Subscriptions
- Customer subscriptions show the exact date when their specific plan_id starts.
- If customers downgrade from a pro plan or cancel their subscription - the higher plan will remain in place until the period is over - the start_date in the subscriptions table will reflect the date that the actual plan changes.
- When customers upgrade their account from a basic plan to a pro or annual pro plan - the higher plan will take effect straight away.
- When customers churn - they will keep their access until the end of their current billing period but the start_date will be technically the day they decided to cancel their service.
- 
#### Solution
  **I have carefully provided my solutions to the four parts of the case study in this repository( see the [jupyter notebook file](https://github.com/DataStance1/Foodie_fi_SQL_Case_Study_Solution/blob/main/Foodie_Fi_SQL_Case_Study_Solution_by_Caleb_Ugorji.ipynb))** 
- See the summary dashboard here [Foodie_fi_summary_dashboard](https://public.tableau.com/app/profile/caleb.chijindu.ugorji/viz/Foodie_fisummarydashboard/Dashboard3?publish=yes) 

*Thank you for your time. I would appreciate your feedback*
