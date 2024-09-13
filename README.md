## Book Recommendation System

### Data Description   
We've three dataset -  
• Book data – (ISBN, Book-Title, Book-Author, Year-Of-Publication, Publisher, Image-URL-S, Image-URL-M, Image-URL-L)  
• Users data - (User-ID, Location, Age)  
• Ratings data - (User-ID, ISBN, Book-Rating)   

Dataset link:
Books.csv: https://drive.google.com/uc?export=download&id=1jlbf103aeTHKUZNdJ2rQd9WXw6hbCqSQ <br>
Ratings.csv: https://drive.google.com/uc?export=download&id=1v4R2uXsoVTfUowMMNhuiMnfdshssL7sv<br>
Users.csv: https://drive.google.com/uc?export=download&id=1Qn0L1vKN5feZxQU2PzNHG9uUr8fUaGh<br>

### Summary of Project

- As the first step, we performed data preparation (i.e data cleaning and feature engineering) and EDA part.   

- After data preparation, build a recommendation system based on popularity (i.e ratings). These recommendations are usually given to every user irrespective of personal characterization. Merged book_data dataset and ratings, considering ISBNs that were explicitly rated for this recommendation system. We have listed all the top 50 books with the highest average rating but we have only selected those books whose no ratings are more than 250.

- The third step is to do Collaborative Filtering - Memory based approach was our first trial on train and test dataset which uses the memory of previous user's interactions to compute user's similarities based on items they’ve interacted with (i.e user-based approach) or compute items similarities based on the users that have interacted with them (i.e item-based approach). Our approach here is that we will only select users who have rated more than 200 books and we will only select books that are rated by more than 50 users to get more accurate results for the model and avoid outliners. Then we apply cosine similarity to make item similarity need to take the transpose of a matrix. This matrix would help in managing the train-test matrix. After all views predictions based on similarity, we find recommendation on it based on score. 

- The last step is to create a function recommend which will take the book name as input from the user and it will return 4 similar books with the author.

### Reference images  
<div align="center">
  <img src="https://github.com/user-attachments/assets/0d35f734-b630-4f8d-949e-4740b0a3da6c" alt="Home" width="400" height="400">
  <img src="https://github.com/user-attachments/assets/bc0a5880-cfdf-40e3-bf52-8f3c4593344d" alt="Top books" width="400" height="400">
</div>
<div align="center">
  <img src="https://github.com/user-attachments/assets/bf917af8-3321-4179-b64e-97385ff22d47" alt="User Query" width="400" height="400">
  <img src="https://github.com/user-attachments/assets/ee4a730f-30b9-47e4-8b15-7b44dcb54624" alt="Result" width="400" height="400">
</div>
