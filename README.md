# Deep Learning-based Recommender Systems

### INTRODUCTION

Recommender Systems are a crucial component of many modern online services, enabling personalized recommendations for products, services, or content. They rely on algorithms that analyze user data to generate personalized recommendations. There are several types of Recommender System algorithms, including collaborative filtering, content-based filtering, and hybrid approaches.

One traditional algorithm used for collaborative filtering is Matrix Factorization, which involves decomposing a user-item interaction matrix into lower dimensional matrices, enabling the generation of recommendations based on similarities between user and item factors.

However, one of the challenges in Recommender Systems is dealing with implicit feedback data, where user interactions with items are not explicitly stated as positive or negative feedback. In these cases, traditional algorithms may not be as effective, and alternative methods are needed.

One such alternative is the Neural Collaborative Filtering (NCF) architecture. NCF is a deep learning-based approach that leverages neural networks to model user-item interactions and make recommendations. It addresses the challenges of implicit feedback data by incorporating non-linear interactions between user and item features, enabling more accurate recommendations. NCF has shown promising results in both accuracy and efficiency in various applications and is becoming increasingly popular in the field of Recommender Systems.

Arxiv: https://arxiv.org/pdf/1708.05031.pdf

### EVALUATING A RECOMMENDER SYSTEM

Hit ratio at k is a commonly used metric for evaluating Recommender Systems. It measures the percentage of recommendations that are relevant to the user among the top k items recommended.

To calculate the hit ratio at k, the recommender system generates a list of k items that it recommends to the user, and then checks how many of these items the user actually interacted with or found relevant. If at least one item in the list is relevant, the recommendation is considered a hit.

For example, let's say a recommender system generates a list of 10 recommended items for a user, and only 3 of them are relevant to the user's interests. If we consider the top 5 recommendations, the hit ratio at 5 would be 0, since none of the relevant items were included in the top 5 recommendations. However, if we consider the top 10 recommendations, the hit ratio at 10 would be 0.3 (3 out of 10 items).

Hit ratio at k is a useful metric for evaluating Recommender Systems because it takes into account the fact that users may not interact with or find all recommended items relevant. It also considers the order in which the items are recommended, which is important in practice as users may not look at all recommended items and may only consider the top few recommendations.

However, it has some limitations, such as not taking into account the rank of the relevant items or their relevance score. It also does not consider the diversity of the recommended items, which is an important aspect of Recommender Systems. Therefore, it is often used in combination with other metrics, such as precision, recall, and diversity measures, to provide a more comprehensive evaluation of the system.
