# Book Advisory - (Book Recommendation System)

## Project Overview
This project implements a book recommendation system using three datasets: Books, Users, and Ratings. The system offers both popularity-based recommendations and collaborative filtering techniques, helping users discover books they are likely to enjoy based on their preferences or the preferences of others with similar tastes.

## Features
- **Data Preparation**: Data cleaning, feature engineering, and exploratory data analysis (EDA) for preprocessing.
- **Popularity-based Recommendations**: Recommends top-rated books with a minimum number of ratings.
- **Collaborative Filtering**: Uses a memory-based approach for user and item similarity to offer personalized recommendations.
- **Recommendation Function**: Recommends similar books based on user input.
  
## Architecture
1. **Data Preparation**: Cleans and merges datasets (Books, Users, Ratings) for effective recommendation generation.
2. **Popularity-based Recommendations**: Lists top-rated books that have been rated by more than 250 users.
3. **Collaborative Filtering**: Uses cosine similarity to compute similarities between books and users.
4. **Recommendation Function**: Provides book recommendations based on user-input book titles.
<div align="center">
  <img src="https://github.com/user-attachments/assets/18d04e6b-e607-44d5-8f44-7d4d3e09e171" alt="Flow Chart" width="700" height="450">
</div>

## Architecture
1. Download the datasets:
   - [Books.csv](https://drive.google.com/uc?export=download&id=1jlbf103aeTHKUZNdJ2rQd9WXw6hbCqSQ)
   - [Ratings.csv](https://drive.google.com/uc?export=download&id=1v4R2uXsoVTfUowMMNhuiMnfdshssL7sv)
   - [Users.csv](https://drive.google.com/uc?export=download&id=1Qn0L1vKN5feZxQU2PzNHG9uUr8fUaGh)

2. Install the required libraries:
   ```bash
   pip install pandas numpy sklearn
3. Run the main script:
   ```bash
   python app.py
### Reference images  
<div align="center">
  <img src="https://github.com/user-attachments/assets/0d35f734-b630-4f8d-949e-4740b0a3da6c" alt="Home" width="500" height="450">
  <img src="https://github.com/user-attachments/assets/bc0a5880-cfdf-40e3-bf52-8f3c4593344d" alt="Top books" width="500" height="450">
</div>
<div align="center">
  <img src="https://github.com/user-attachments/assets/bf917af8-3321-4179-b64e-97385ff22d47" alt="User Query" width="500" height="450">
  <img src="https://github.com/user-attachments/assets/ee4a730f-30b9-47e4-8b15-7b44dcb54624" alt="Result" width="500" height="450">
</div>

### Usage
- Run the system and enter a book name to receive personalized recommendations based on similarity.
- The system provides top-rated books for users based on their preferences and ratings.

### Applications
- Personalized book recommendation platforms.
- Generalized recommendation systems for online bookstores or libraries.
