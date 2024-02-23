# Movie Script Recommender System

## Overview
This project aims to build a recommendation system for movies based solely on their scripts. Unlike traditional recommendation algorithms that rely on user data, this system utilizes the content of the movies to suggest similar films.

## Getting Started
To get started, you'll need to obtain the movie scripts. Refer to the README file to find the resources for obtaining this data. Once you have the scripts, place them in a directory named "scripts" in the project directory.

## Installation
This project requires the following dependencies:
- pandas
- numpy
- tqdm
- gensim
- scikit-learn

You can install these dependencies using pip:
```
pip install pandas numpy tqdm gensim scikit-learn
```

## Usage
1. Run the script to import the movie scripts and convert them into vectors using Doc2Vec.
2. Optionally, you can choose between two formats of the dataset: one where each column represents a vector feature (dfscript), and another where one column holds the entire vector (dfvectors).
3. Define functions for calculating cosine similarity and finding similar movies.
4. Optionally, perform clustering using KMeans to group similar movies.
5. Utilize the recommendation function to suggest movies based on the input.

### Example Usage:
```python
recommend(['No Country for Old Men', 'Mean Girls'])
```

## Conclusion
By leveraging clustering and mathematical methods, this project demonstrates the creation of a recommendation system without relying on user data. While the algorithm works effectively, there are areas for improvement, such as recommending movies from multiple clusters and handling duplicates. Future iterations may address these issues for enhanced performance.
