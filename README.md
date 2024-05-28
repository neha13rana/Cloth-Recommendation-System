# Cloth-Recommendation-System

We have chosen a fashion dataset for our system. We've created a clothing recommendation system using data mining and content-based filtering concepts. Customers can input a cloth ID and receive details on the top 5 related clothing items.
**Steps :**
1) Download the ipynb file in your system.
2) Run on kaggle/any suitable platform.
3) Enter the Cloth ID by which you want related cloth.
4) In output you will get top5 recommended clothes details.


**Proposed Algorithm :**

![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/4234e9f3-b579-4910-897c-6d835603f7e0)

**1) Dataset Description :**
We have selected a fashion dataset openly available on hugging face. The
dataset consists of various features that describe a cloth. The clothes mentioned in
the dataset are from different brands that have different master, sub-categories, and
colors. They are worn in different seasons and were launched in different years. All
these along with some more features make this dataset a useful source for building
a content-based recommendation system.
Source link : https://huggingface.co/datasets/ashraq/fashion-product-images-small

**2) Novelty :**
The recommendation systems are a well-liked and extensively employed
method for giving customers customized recommendations. There are different
types of recommendation systems algorithms based on data available. The one that
we have used in this project is :
 1. Content-Based Filtering Recommendation System
 2. Weighted Word2vec


**3) Result :**
  Output 1 :
  ![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/fff26be5-37d5-47fb-8215-5c0c0682a811)

  Output 2 :
  ![Uploading image.png…]()


4) Conclusion :
The above output shows that the result produced by BOW and Weighted
Wrd2Vec does not differ much.
To evaluate the performance of this system either we need to have labeled
data or we can use any of the below methods :
• User Feedback Collection: Gather feedback from users through surveys or
studies to understand their perception of the recommended items’ relevance
and utility. This qualitative input helps assess the system’s effectiveness.
• A/B Testing Method: Conduct A/B testing by dividing users into different
groups to compare the performance of the recommendation system against
alternatives or no recommendations at all. Analyze user engagement metrics
like click-through rates to measure impact.
• Implicit Signals Analysis: Utilize implicit feedback cues such as user interactions (e.g., clicks, purchases) to infer user preferences and evaluate how well
the recommendation system aligns with user behavior.
To conclude, the choice of the approach depends on Tag size and the computation power available. If the tag size is large such that the weighted wrd2vec vector
is smaller than the BOW vector then we can go for weighted wrd2vec, or else with
BOW.



