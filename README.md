# CMPE260_RL_BookRecommendations

## Deep Reinforcement Learning based Recommendation System
Develop a reinforcement learning-based book recommendation system that employs deep deterministic policy gradients. The system should effectively leverage actor-critic networks to dynamically adapt to user preferences, optimizing recommendations through continuous interactions. Implement exploration-exploitation strategies like Gaussian and Ornstein-Uhlenbeck noise to fine-tune the policy, ensuring personalized and evolving book suggestions for users. The qualitative evaluation will gauge the efficacy of book recommendations by assessing their alignment with users' past interactions, considering factors such as genre, language, and the book's status as a best seller. 

#### Dataset
This system recommends books to user based on the user's past interactions (ratings) with books. 

Data source: <br>
[Book Recommendation Dataset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset?select=Books.csv) <br>
[Curated dataset](https://drive.google.com/drive/u/1/folders/1DOsnhjb9-Uvy8dvbijbkSvhvasxZH_yE)

#### Trained models
1. [Base](https://drive.google.com/drive/u/1/folders/1uebck-GkeVgaAqh6TazuyzJxIdNFTVm3) - uses user and book embeddings to model user-book interactions
2. [Base + user demographic features](https://drive.google.com/drive/u/1/folders/13EEajIp5AtYhZ3ceG6mCZRgzaHI-CN5i) - incorporates user features like location and age into the embeddings 
3. [Base + OU noise](https://drive.google.com/drive/u/1/folders/1phCZETFhn4HGxYi8JOaIwkjjHDmG3mT5) - time-correlated noise is added to the actions taken by the deterministic policy
4. [Base  + Gaussian noise](https://drive.google.com/drive/u/1/folders/16Xd1T3Wq-0UDbdQVDsuh66uFgE9FiU7y) - gaussian noise is added to the actions

#### Reference: 
Paper - [Deep Reinforcement Learning based Recommendation with Explicit User-Item Interactions Modeling](https://arxiv.org/pdf/1810.12027.pdf) <br>
Implementation - [Github](https://github.com/shashist/recsys-rl/tree/master)

