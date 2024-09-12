# 🎥 **The Netflix Recommendation System**
Recommend the similar movie(s) or TV show(s) based on Cosine Similarity algorithm.
![cover](materials/cover.jpg)

## ✍ Description:
- Netflix is one of the most popular streaming platforms with a vast library of movies and TV shows spanning various genres. With so many options, making a decision can often feel overwhelming. This recommendation system helps users by suggesting similar content based on their favorite movies or shows. Using a combination of Term Frequency-Inverse Document Frequency (TF-IDF) and Cosine Similarity, it finds content with the highest similarity to what the user likes, making selection easier and more enjoyable.
- The dataset 'netflix_data.csv' contains: 12 columns which describing the title, country, description,...and 8807 rows belong to each of the movies/TV show.


## ✪ Usage:
### The project is designed to be completeted these following steps:
**1. Data collecting:** Download the dataset from Kaggle platform [here](https://www.kaggle.com/datasets/ashfakyeafi/netflix-movies-and-shows-dataset)
**2. Data preparation:**
   - Take an overall look the dataset.
   - Cleaning data: Fill the missing values
**3. Exploration Data Analysis:**
   - Visualize the distribution of the contents regarding the movies/TV shows such as the rating, the countries to understand trends in content production and viewer preferences.
   - Genarate the images of the common words in the description as well as the listed-in.
**4. Feature Engineering:**
Text cleaning is essential to standardize and simplify the input data, ensuring more accurate analysis during the TF-IDF transformation.
   - Create a class TextCleaner combinding several steps to cleaning the text:
     a. Seperate text
     b. Remove space
     b. Remove punctuation characters
   - Create the BAG OF WORDS of each the objects to calculate.
**5. The TF-IDF and Cosine Similarity:**
   - After we generate a new dataframe containing 2 columns: Type and BagOfWords:
     a. Transforming the value BagOfWords into the matrix by using TfidfVectorizer()
     b. Calculating the similarity among the words of matrix by using Cosine-similarity formula.
     c. Save the results of the matrix, the cosine-similar into our files and the new dataframe we made from it.

**6. Build the recommendation system:**
  -  Create the class Netfixrec: sorting the values 'similarity' we calculated previously to yeild the list of the similar movie(s) or TV show(s).
  -  Output the result.
# 🗳️ The sample results:
The movie/Tv show title: dick johnson is dead
Similar Movie(s) list:
1. How to Be a Player
2. End Game
3. Midnight Special
4. The Death and Life of Marsha P. Johnson
5. Small Soldiers
6. Woodshock
7. A Gray State
8. Win It All

Similar TV show(s) list:
1. New Girl
2. Barbie Dreamhouse Adventures

   
## 💻 Method:
- Content Based Filtering- They suggest similar items based on a particular item. This system uses item metadata, such as genre, director, description, actors, etc. for movies, to make these recommendations. The general idea behind these recommender systems is that if a person liked a particular item, he or she will also like an item that is similar to it.

  

## 🔖 Credits and Acknowledgements:
- Ashfak Yeafi: This project was inspired by Asfak Yeafi's work on Kaggle. His project provided valuable steps and served as a reference point in the development of this project. You can view his original work [here](https://www.kaggle.com/code/ashfakyeafi/movie-recommendation-system).



