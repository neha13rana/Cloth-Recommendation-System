# Cloth-Recommendation-System

We have developed a cloth recommendation system using content-based filtering. Representing cloth tags numerically using Bag of Words and Word2Vec. For Word2Vec, we use TF-IDF to weight individual word vectors. To optimize the system, we implemented Sparse Cosine similarity, as tags have at most 10 words and there are around 1600 unique words, improving complexity. With 44,000 samples, precalculating the similarity matrix is impractical for low-end devices due to space and time overhead. By dynamically calculating similarity at query time using sparse operations, we maintain similar running time complexity with reduced space overhead.

<hr>

**Steps :**
1) Download the ipynb file in your system.
2) Run on kaggle/any suitable platform.
3) Enter the Cloth ID by which you want related cloth.
4) In output you will get top5 recommended clothes details.

<hr>

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

**2) Data visualization:**

![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/e417b827-bd11-494c-aacc-0dfa7e902386)

![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/cb88895f-f4f9-4fbe-a0bb-8e69c1453fb3)

![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/0d3762f4-f368-431e-9bb4-26bd2af586b6)

![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/ad0a4a72-c369-4794-b2de-bb59fc5816ca)


**3) Novelty :**
The recommendation systems are a well-liked and extensively employed method for giving customers customized recommendations. There are different types of recommendation systems algorithms based on data available. The one that we have used in this project is :
 
**Content-Based Filtering Recommendation System-** 
It recommends items similar to those a user has liked or interacted with in the past. It analyzes the attributes or features of items and recommends items with similar characteristics. We have compared the results of the recommendation made by using two different approaches to vectorizing the features.


**4) Result :**
  """
  Output 1 :
  
  ![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/fff26be5-37d5-47fb-8215-5c0c0682a811)

  Output 2 :
  
  ![image](https://github.com/neha13rana/Cloth-Recommendation-System/assets/121093178/0eaa9ce3-f916-4315-9fb9-a38314f65b68)


**5) Conclusion :**
The above output shows that the result produced by BOW and Weighted Wrd2Vec does not differ much.

To evaluate the performance of this system either we need to have labeled data or we can use any of the below methods :

• **User Feedback Collection:** Gather feedback from users through surveys or studies to understand their perception of the recommended items’ relevance and utility. This qualitative input helps assess the system’s effectiveness.

• **A/B Testing Method:**  Conduct A/B testing by dividing users into different groups to compare the performance of the recommendation system against alternatives or no recommendations at all. Analyze user engagement metrics like click-through rates to measure impact.

• **Implicit Signals Analysis:**  Utilize implicit feedback cues such as user interactions (e.g., clicks, purchases) to infer user preferences and evaluate how well the recommendation system aligns with user behavior.
 
To conclude, the choice of the approach depends on Tag size and the computation power available. If the tag size is large such that the weighted wrd2vec vector
is smaller than the BOW vector then we can go for weighted wrd2vec, or else with
BOW.


**Contributors -** 

 - [neha13rana](https://github.com/neha13rana)
 - [Priya-1543](https://github.com/Priya-1543)
 - [Kushpurohit23](https://github.com/Kushpurohit23)
