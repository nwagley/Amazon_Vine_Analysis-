# Amazon_Vine_Analysis-
## Purpose 
The purpose of this project is to analyzes Amazon Vine program and find out if there is a bias towards vine memebers and their review. We will firstly create a cloud relational database using Amazon Web Services (AWS) and connected our database using a PostgreSQL. After this PostgreSQL is done then we will create four tables in our RDS using the schema provided. At the end of Deliverable 1, We will extracted Amazon review dataset regarding video game reviews which I have chosen then transforme the data based on the directions provided for the Challenge and then uploaded the data into our cloud database tables. We used postgreSQL to create our tables and PySpark for the ETL process. 
## Result
<img width="788" alt="upload written" src="https://user-images.githubusercontent.com/79885849/122696350-1b03d100-d200-11eb-9f75-308df7785464.PNG">

After this step if finished we again extracted video game Amazon review datasets and loaded the data into a new GoogleColab notebook using PySpark. We filtered the data to only include games where total reviews received were greater than 20. We then further filtered the data to include games where the proportion of helpful votes to total is greater than or equal to 50%. Finally we divded the dataset into two groups: reviews given as part of the vine program(paid) and reviews given oustide the vide program(unpaid). Using the two datasets, we compared the ratio of proportion of 5-star reviews to total reviews between reviews obtain from the vine program and reviews outside the vine program. Our Analysis Code for this exercise is also included in this repository.

<img width="224" alt="1" src="https://user-images.githubusercontent.com/79885849/122697465-a716f800-d202-11eb-8d80-7d9101667097.PNG"> <img width="252" alt="2" src="https://user-images.githubusercontent.com/79885849/122697467-a7af8e80-d202-11eb-9b73-f4418ebd9ab3.PNG">

## Conclusion 

From the above table and screenshot we can read that when comparing 5-star ratings between the two datasets there is a significant increase in 5-star reviews when reivews are obtained from the Vine Program. This tells us that the company a positive bias for reviews within the vine program. We could perform further analysis into this data which would compare the proportion of all the ratings instead of only focusing on 5-star ratings. After this conclusion we can then provide a better picture on whether a bias exists accross all ratings and not just the top rating. We could also compare the average rating within the two data sets  to determine if there is a general probability of reviewers providing better reviews within the vine program.

<img width="479" alt="3" src="https://user-images.githubusercontent.com/79885849/122697518-bdbd4f00-d202-11eb-97dd-f1ad72a095ac.PNG">
