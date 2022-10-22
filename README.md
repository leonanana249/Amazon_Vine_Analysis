# Amazon_Vine_Analysis

## Overview of the analysis
Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.<br/>
In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.<br/>

Results 
•	How many Vine reviews and non-Vine reviews were there?<br/>

![image](https://user-images.githubusercontent.com/107721712/197361992-b1d181ad-f39f-4e42-91eb-ef068c7f5e71.png)<br/>
•	How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?<br/>
![image](https://user-images.githubusercontent.com/107721712/197362043-28baffe5-1fd6-4289-94a3-790869684a85.png)<br/>
•	What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?<br/>
![image](https://user-images.githubusercontent.com/107721712/197362026-2a0676fc-3f02-4036-8679-44e02188f686.png)<br/>
## Summary 
The analysis tends not to have positivity bias because the helpful is pre-determined by the total votes greater than or equal to 20. There could be more 5-star reviews when the total votes are below 20. <br/>

### Additional analysis 
If counting the total reviews, there are 149,086 reviews, which is much higher than the helpful reviews of 355.<br/>
![image](https://user-images.githubusercontent.com/107721712/197362472-76144833-3830-4959-8b33-a9097cd0597d.png)<br/>

 Meanwhile, total 5-star reviews are 129,709. <br/>
![image](https://user-images.githubusercontent.com/107721712/197362486-4d9a42d9-4217-482d-8fa1-92fc3fc1e99c.png)<br/>

Moreover,  the Non-Paid 5-star reviews will take up to 100% if we don’t consider helpful threshold. <br/>

![image](https://user-images.githubusercontent.com/107721712/197362508-1aee8522-8175-4b74-9c15-6c8b4c7a19ce.png)<br/>
