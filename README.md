# Amazon_Vine_Analysis

## Analysis Overview
We are given access to over 50 datasets containing product reviews on Amazon that were conducted via the Amazon Vine program. I chose the Video Game review data set to extract the product reviews, created a PostgreSQL database, and inserted the values from my notebook in Google Collab.

Then, since we want to determine if there is a bias via the Amazon Vine program, I created new dataframes in my Google Collab notebook that filtered on video games with at least 20 reviews (to generate a large enough sample size), filtered on reviews that were determined to be at least 50% helpful, and then counted how many 5 star reviews there were of each video game through the paid Vine program and compared to see if there was a difference between the unpaid reviews.

![image](https://user-images.githubusercontent.com/92773195/153771899-b5dbfb96-8853-4b6b-bcca-42a46eaabb21.png)
![image](https://user-images.githubusercontent.com/92773195/153771916-88994d7b-2701-4d4a-8008-93da02bf58e1.png)
![image](https://user-images.githubusercontent.com/92773195/153771921-125eea7f-5c1a-423b-9e1b-915378196a84.png)
![image](https://user-images.githubusercontent.com/92773195/153771927-238bbbf7-84f0-418c-8f9c-618e90436599.png)
![image](https://user-images.githubusercontent.com/92773195/153771936-4f4a8459-6e6e-4a22-a90b-c1ffe766a445.png)
![image](https://user-images.githubusercontent.com/92773195/153771966-ee148203-ae4f-43eb-ba69-51588ad13614.png)
![image](https://user-images.githubusercontent.com/92773195/153771975-ee879ba0-dea9-4af0-a957-6ac8749ca145.png)
![image](https://user-images.githubusercontent.com/92773195/153771983-6b33a742-3882-40e0-a83e-6302499d1756.png)
![image](https://user-images.githubusercontent.com/92773195/153771992-f2f22cf8-30d0-430b-b2a2-fae9cffae82f.png)
![image](https://user-images.githubusercontent.com/92773195/153772001-44876421-6c93-4d50-9234-aa6498d204ba.png)

## RESULTS
1) As we can see from the final image, there were 94 video games reviewed from the paid Vine program, compared to 40471 that were unpaid reviews. 
2) 48 paid vine video games received a 5-star review, while 15663 unpaid video games received a 5-star review
3) Of the 94 paid vine reviews, 51.06% were given a 5-star review. Comparitevly, only 38.7% of unpaid video games received a 5-star review. 

## Summary
Based on my analysis, it certainly appears that the Amazon Vine program causes a certain amount of bias from users who are required to publish a review of the video game product. Since there is approximately a 12.4% increase in 5-star reviews for video games within the Vine program, I believe we can safely conclude there is a certain amount of bias caused by Vine. An additional analysis I would recommend would be to run a 2-sample t-test using R to determine if there is enough evidence to conclude that Vine reviewed products are more likely to receive a 5-star review than their unpaid counterparts. We could also attempt to see if there is a different in average star rating using the same methodology that was displayed above.
