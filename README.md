# SENTIMENT-ANALYSIS-WITH-NLP

*COMPANY* : CODTECH IT SOLUTIONS

*NAME* : CHINTHAPARTHI THISHITHA

*INTERN ID* : CT06DM1408

*DOMAIN* : MACHINE LEARNING

*DURATION* : 6 WEEKS

*MENTOR* : NEELA SANTOSH

The goal of my project was to perform sentiment analysis using Natural Language Processing (NLP) techniques on movie reviews from the IMDb dataset. The objective was to classify the reviews as either positive or negative based on the textual content. This task falls under supervised text classification and is commonly used in real-world applications like opinion mining, product review analysis, and social media monitoring.

To begin the project, I gathered information from various sources such as Google and YouTube. These platforms helped me understand how sentiment analysis works, the steps involved in cleaning text data, and how to implement machine learning models using Python. With the theoretical understanding in place, I downloaded the IMDb Movie Reviews Dataset, which contains 50,000 labeled reviews—half of them positive and the other half negative.

I used Google Colab for coding and experimentation. It allowed me to run Python code in the cloud, which was convenient and efficient. When I initially tried loading the dataset using pandas.read_csv(), I encountered some encoding issues and malformed rows. To handle this, I used encoding='utf-8' and on_bad_lines='skip' to read the file while ignoring corrupted lines. Once the dataset was loaded successfully, I explored it using functions like df.head() and df.shape() to understand the structure.

The next step involved preprocessing the textual data. Raw text is usually messy and not suitable for machine learning models in its original form. I created a preprocessing function using regular expressions to remove HTML tags and non-alphabetic characters. I converted the text to lowercase to maintain consistency. Then, I added NLTK-based preprocessing, which included removing stopwords (commonly used words like "the", "is", etc.) and applying lemmatization to reduce words to their base form (e.g., "running" to "run"). These steps helped reduce noise and improved the quality of features used for training the model.

After preprocessing, I transformed the cleaned text data into numerical features using TF-IDF Vectorization. I set the maximum number of features to 5000 to reduce dimensionality while capturing important terms. This transformation resulted in a matrix suitable for feeding into a machine learning model.

For the classification task, I used Logistic Regression, a simple yet powerful algorithm suitable for binary classification problems like sentiment analysis. I split the dataset into training and testing sets using an 80:20 ratio and trained the model on the training data. Predictions were made on the test set, and I evaluated the model using multiple performance metrics.

The model achieved an accuracy of over 87%, which indicates strong performance. I also printed a classification report that included precision, recall, and F1-score for both classes. To visualize the performance, I used a confusion matrix with Seaborn heatmap using a mako color palette, which made it easy to interpret true vs. false predictions. Additionally, I calculated the ROC AUC score, which showed how well the model distinguishes between positive and negative reviews across various thresholds.

In conclusion, this project provided hands-on experience with NLP, text preprocessing, and classification using machine learning. From data collection to model evaluation, I went through every essential step of an NLP pipeline. Learning through real datasets and addressing practical issues like encoding and preprocessing gave me a deeper understanding of how sentiment analysis systems are built. This project not only strengthened my Python and machine learning skills but also demonstrated how NLP can be applied effectively to understand human emotions and opinions through text.


