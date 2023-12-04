# CMPE260_RL_BookRecommendations

## Deep Reinforcement Learning based Recommendation System
Recommendation systems play a pivotal role in any content based industry. A variety of techniques like collaborative filtering, matrix factorization based methods etc have been used. However there are two prevalent challenges:
1. The dynamic interaction between users and recommender systems is ignored  and recommendation is seen as a static activity.
2. They ignore the long-term advantages in favour of focusing primarily on the instant reaction from recommended items.

We tackle these challenges by modeling the user interactions with the system by treating recommendation as sequential decision making process. We use Actor-critic reinforcement technique, hence taking into account the long term benefits and dynamic adaptation.

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

