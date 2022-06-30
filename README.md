# Amazon_Vine_Analysis

### Purpose

The purpose of this project is to analysis the Amazon review Vine program on a certain product to determine if there is any bias toward favorable reviews by Vine members. We will take a product and analyze the data by using Google Colab to read in the data from Amazon’s Simple Storage Service (S3). Using this data we will give the SellBy Stakeholders an analysis determining whether Amazon’s Vine program creates a bias for products.

### Results

In order for us to determine if there is a bias of Vine reviews, we created a dataframe from our Amazon review data that had these 6 columns.

  1. review_id: The unique ID of the reviewer.
  2. star_rating: The 1-5 star rating og the review.
  3. helpful_votes: Number of helpful votes.
  4. total_votes: Number of total votes the review received.
  5. vine: Review was written as part of the Vine program.
  6. verified_purchase: The review is on a verified purchase.
  
We filtered the dataframe to retrieve rows where the total_count was greater or equal to 20, we also filtered to show reviews that are more likely to be helpful. We also created 2 more dataframes to determine if they where a Vine (paid) or a non-Vine (unpaid) review.

#### Total Number of Reviews

Vine Reviews

![Number of reivews paid](https://user-images.githubusercontent.com/100821974/176732854-cabf8f5a-f03f-42d4-b845-53684844b601.png)

Non-Vine Reviews

![Number of reviews unpaid](https://github.com/Tony-Lew/Amazon_Vine_Analysis/blob/main/Resources/Number%20of%20%20reivews%20unpaid.png)

#### Number of 5 Star Reviews

Vine 5 Star Reviews

![Number of 5 star reviews paid](https://github.com/Tony-Lew/Amazon_Vine_Analysis/blob/main/Resources/Number%20of%205%20star%20reivews%20paid.png)

Non-Vine 5 Star Reviews

![Number of 5 star reviews unpaid](https://github.com/Tony-Lew/Amazon_Vine_Analysis/blob/main/Resources/Number%20of%205%20star%20reivews%20unpaid.png)

#### Percentage of 5 Star Reviews

Vine 5 Star Reviews Percentage

![Percentage of 5 star reivews paid](https://github.com/Tony-Lew/Amazon_Vine_Analysis/blob/main/Resources/Percentage%20of%205%20star%20reivews%20paid.png)

Non-Vine 5 Star Percentage

![Percentage of 5 star unpaid](https://github.com/Tony-Lew/Amazon_Vine_Analysis/blob/main/Resources/Percentage%20of%205%20star%20unpaid.png)

### Summary

Reviewing the results of the Vine and Non-Vine data, It shows that the Non-Vine reviews where higher than the Vine Reviewed. The Non-Vine Reviewers gave it a 5 star at 53% where the Vine Reviewers gave it a 5 Star at 42%. These numbers are very scewed as the Vine reviews is less then 1% of total reviewers compared to the Non-Vine Reviewers.
