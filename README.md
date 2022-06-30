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
