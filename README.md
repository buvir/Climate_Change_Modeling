📘 Climate Change Modeling – Machine Learning Project
📌 Project Overview

This project applies Data Science and Machine Learning techniques to analyze public discourse on climate change using comments collected from NASA’s Climate Change Facebook page.
The goal is to explore engagement patterns, preprocess text data, and build a predictive model to estimate user engagement based on comment content and metadata.

The project follows a complete end-to-end data science workflow, from exploratory data analysis to model evaluation and interpretation.

🛠️ Tools & Technologies Used

Programming Language: Python

IDE: VS Code (Jupyter Notebook)

Libraries:

pandas

numpy

matplotlib

seaborn

scikit-learn

scipy

re (regex)

📂 Project Structure
Climate-Change-Modeling/
│
├── climate_nasa.csv          # Dataset
├── Climate_Change_Modeling.ipynb  # Jupyter Notebook (main file)
├── README.md                 # Project documentation

📊 Dataset Description

Source: NASA Climate Change Facebook Page

Time Range: 2020 – 2023

Total Records: 522 comments

Columns:
Column Name	Description
date	Date and time of comment
likesCount	Number of likes received
commentsCount	Number of replies
profileName	Anonymized user identifier
text	Original comment text

All user identities are anonymized in compliance with ethical data handling practices.

🧩 Project Workflow (As per PDF – Fully Covered)
1️⃣ Problem Understanding

Defined the challenge of modeling climate-related public engagement.

Framed the task as a regression problem predicting likes count.

2️⃣ Dataset Preparation

Loaded and inspected the dataset.

Verified data types and structure.

Generated statistical summaries.

3️⃣ Exploratory Data Analysis (EDA)

Charts included:

Missing values bar chart

Distribution of likes count

Distribution of comments count

Likes vs comments scatter plot

Comment text length distribution

Key insights identified:

Engagement metrics are highly skewed.

Majority of comments receive low interaction.

Few comments act as outliers with very high likes.

4️⃣ Data Preprocessing

Handled missing values:

commentsCount → filled with 0

text → filled with empty string

Converted date to datetime format.

Created time-based features:

year, month, day

Cleaned text using:

Lowercasing

URL removal

Punctuation removal

Extra space normalization

5️⃣ Feature Engineering

Created text_length feature.

Applied TF-IDF Vectorization on cleaned text.

Combined:

Text features (1000 dimensions)

Numeric features (commentsCount, text_length, year, month)

6️⃣ Model Selection & Training

Model Used: Random Forest Regressor

Reason:

Handles non-linear data

Robust to noise

Widely accepted for regression tasks

Train-test split: 80% / 20%

7️⃣ Model Evaluation

Metrics reported:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score

Visualization included:

Actual vs Predicted Likes Count scatter plot

📌 Note: Low R² is expected due to the unpredictable nature of human social media behavior.

8️⃣ Conclusion

Demonstrated that engagement prediction is challenging due to external factors.

Highlighted the importance of proper preprocessing and honest evaluation.

Emphasized methodology over overfitting.

9️⃣ Future Scope

Sentiment analysis

Topic modeling

Emotion detection

Transformer-based NLP models (BERT)

Inclusion of post-level metadata

📈 Charts & Visualizations Included

✔ Missing Values Bar Chart
✔ Likes Count Distribution
✔ Comments Count Distribution
✔ Likes vs Comments Scatter Plot
✔ Text Length Distribution
✔ Actual vs Predicted Output Plot


▶️ How to Run the Project

Clone or download the project folder

Install required packages:
```

pip install pandas numpy matplotlib seaborn scikit-learn scipy

```
Open Climate_Change_Modeling.ipynb in VS Code

Run cells sequentially from top to bottom

📌 Final Notes

This project is suitable for:

Academic submission

Final-year project

Data Science portfolio

NLP demonstration project

The focus is on correct methodology, transparency, and real-world data challenges, fully aligned with the provided project specification.


