## Building a grocery recommendation system using association rules and graph ML techniques
Specifics of model training:
I tried out 2 approaches:

a. Association Rules:

Data Preparation: The input is a transaction dataset (mentioned as basket in the code) where each transaction contains a list of items bought together. 
Model Training:
- Frequent Itemsets Generation: Use algorithms like Apriori or FP-Growth to find frequent itemsets (sets of products that appear together in transactions above a specified support threshold).
- Rule Generation: Generate association rules from the frequent itemsets. Each rule has an antecedent (if) and a consequent (then) with metrics like support, confidence, and lift.
Output: A set of association rules that can be used for making recommendations.


b. Graph-Based Recommendations using Jaccard Coefficient:
Data Preparation: The input is a transaction dataset where each transaction         contains a list of items bought together.
       2. Model Training:
Graph Construction: Built a graph where nodes represent products and     edges represent co-occurrence of products in transactions. The weight of an edge is the number of times the two products appear together.
     3. Output: A graph with nodes and weighted edges representing product   co-occurrences.

