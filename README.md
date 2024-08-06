**Customer Review Prediction using NLP by building a TF-IDF Vectoriser**

**Dataset:** https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews
Comprises reviews from a Product based Company. It encompasses a time span of over 10 years, including approximately 500,000 reviews up until October 2012. Each review includes product and user information, ratings, and a plain text review. 

**Action plan**

- Import libraries.
- Load the dataset.
- Remove all observations where the reviews are "Neutral" based on the score value.
- Replace the values of the score column with "Positive" or "Negative" based on the score value.
- Write the code to remove duplicates from the data and remove the rows where the Helpfulness Numerator is greater than the Helpfulness Denominator.
- Store the resulting dataframe in a variable called "Updated".
- Calculate TF-IDF.

The dataset contains the following attributes: 
 Id
ProductID
UserId
Profilename
HelpfullnessNumerator
HelpfulnessDenominator
Score (Rating between 1 and 5)
Time (Timestamp for the review)
Summary (Brief summary of the review)
Text (Text of the review)
 
- In this dataset, the score column has five possible values: 1, 2, 3, 4, and 5. We can consider scores 1 and 2 as negative reviews, scores 4 and 5 as positive reviews, and score 3 as neutral. To predict whether a review is positive or negative, we can remove the neutral reviews.
- The Helpfulness Numerator indicates the number of people who found the review useful, while the Helpfulness Denominator represents the count of useful reviews plus the count of not-so-useful reviews.
- From this information, we can observe that the Helpfulness Numerator is always less than or equal to the Helpfulness Denominator. 

