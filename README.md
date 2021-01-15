# Music_Recommendation
A Comparison of Neighborhood-Based and Latent Factor-Based Collaborative Filtering for Music Recommendation

## Abstract
We compare two collaborative filtering approaches for recommending music based on a set of implicit feedback(such as a listen count) a neighborhood approach and a latent model approach. We compare our results from these approaches with a third naive popularity recommender as a baseline. 
Our results found that the latent model approach performs the best while the neighborhood and popularity approach are roughly equal.

## Methodology
  A. Popularity-based Approach
  B. User-based Neighborhood Approach
      Our goal is to predict the unobserved rating r_ui a user u might give an item i. We denote U as the set of k nearest users to u who rated i. The value
      of rui is a weighted average. This is a traditional k-nearest neighbors approach.
  C. Latent Factor Approach
      We lay out our m users and n items in a n × m ”interaction” matrix where each value r_ui denotes the rating user u has given item i. This rating is implicit 
      such as the number of times the user has listened to that song. Second, we decompose this interaction matrix into an m × f matrix X and an n × f matrix Y 
      where f is the number of latent factors. Then to predict a user’s rating for a certain item, we take the inner product. 
     
## Results    
      ![test]("https://github.com/TiffanySirui/Music_Recommendation/blob/main/results/ROC_Neighborhood_method.png")
