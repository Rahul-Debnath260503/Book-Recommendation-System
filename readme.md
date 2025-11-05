
# Book Recommendation System Project

## Project Goal:

The goal of this project was to build a recommendation system to suggest books to users based on their ratings and book popularity.

## Project Steps:

1.  **Data Loading**: Loaded the "Books.csv", "Ratings.csv", and "Users.csv" datasets into pandas DataFrames.
2.  **Data Preprocessing**:
    *   Checked for missing values in each dataframe.
    *   Merged the three dataframes based on 'ISBN' and 'User-ID'.
    *   Handled missing values in the merged dataframe by imputing 'Age' with the median and dropping rows with missing values in 'Book-Author', 'Publisher', and 'Image-URL-L'.
3.  **Exploratory Data Analysis (EDA)**:
    *   Visualized the distribution of book ratings.
    *   Identified and displayed the top 10 most active users (based on the number of ratings).
    *   Identified and displayed the top 10 most popular books (based on the number of ratings).
4.  **Building Recommendation Models**:
    *   **Popularity-Based Model**: Built a popularity-based recommendation model by calculating the average rating and rating count for each book. Filtered for books with a minimum number of ratings and sorted by average rating to identify popular books.
    *   **Collaborative Filtering Model**: (Planned but not yet fully implemented in the provided notebook) This model aims to provide personalized recommendations based on user-item interactions.
5.  **Displaying Sample Recommendations**: Displayed a sample recommendation list using the built popularity-based model.

## Key Findings from EDA and Popularity Model:

*   The rating distribution showed a high number of 0 ratings, indicating implicit ratings or unrated books.
*   Identified users who have provided a significant number of ratings.
*   Identified books that have received the most ratings.
*   The popularity-based model highlighted books with high average ratings among those with a sufficient number of ratings.

## Next Steps (Based on the Original Plan):

*   Complete the implementation and training of the collaborative filtering model.
*   Evaluate the performance of both recommendation models using appropriate metrics.
*   Compare the results of the popularity-based and collaborative filtering models.
*   Potentially explore hybrid recommendation approaches.
