# IT496-T18-CP2

# DOPE-a-MINE(Team-18)
- Maulik Thakkar (202101415)
- Maharshi Pipaliya (202101210)
- Sameer Sonara (202101489)
- Harshil Patel (202101019)
- Kunj Kapadiya (202103018)

# Introduction
This dataset provides valuable insights into the world of books available on a book depository, encompassing a wealth of information, including titles, descriptions, unique identifiers, publication details, and a variety of attributes related to their physical characteristics. One of the significant attributes is the format of these books, which often influences their handling, shipping, and reader experience. The format may range from hardcover to paperback, e-books, and other variants, each tailored to meet different reader preferences and industry demands.


# Columns Present

- **authors** : list of authors
- **bestseller-rank** : Bestseller ranking
- **categories** : List of all categories (genres)
- **description** : Description(string)
- **dimension-x** : Dimension along x axis (float in cms)
- **dimension-y** : Dimension along y axis (float in cms)
- **dimension-z** : Dimension along z axis (float in cms)
- **edition** : Edition (string)
- **edition-statement** : Edition statement (string)
- **for-ages** : Ranges of ages 
- **format** : Format 
- **id** : Unique Identifier
- **illustration-note**
- **image-checksum** : Cover Image checksum
- **image-path** : Cover image file path
- **image-url** : Cover image url
- **imprint**
- **index-date** : Crawling date 
- **isbn10** : ISBN-10
- **isbn13** : ISBN-13 
- **lang** : List of languages of book
- **publication-date** : Publication date
- **publication-place** : Publication place
- **rating-avg** : Rating average (0-5)
- **rating-count** : Number of ratings 
- **title** : Book's title 
- **url** : Relative URL (https://bookdepository.com + url)
- **weight** : Weight of book

# Key Insights

- In this dataset, we encounter a classification challenge wherein we aim to categorize readers into different age groups based on the information provided in the book titles and descriptions. However, it's worth noting that the "for-ages" column, which could have been a valuable source of information for this task, contains a significant number of missing values (as we can see in missing value heatmap), rendering it unsuitable for use in this particular classification problem.
- There is a larger number of books falling into the following categories :
1) Contemporary Fiction
2) Teaching Resources & Education
3) Children Fiction
4) Horror
5) Science Fiction
6) Graphic Novels ,Anime & Manga
7) Anthologies (non - poetry)
8) Study & Learning Skills : General
9) Miscellaneous Items

- The significant formats are Hardback , Paperback ,CD , Audio , Calender , Cards and Spiral. 
- Paperback, Hardback, and CD constitute about 98% of all formats in the dataset. So we will consider only these three formats
- Based on the scatter plots, it's evident that CDs tend to have smaller dimension-z values and are relatively lightweight. In contrast, hardback books exhibit significantly higher weights. Paperback books, on the other hand, fall in between with intermediate dimension-z and weight values.CDs tend to have equal dimension-x and dimension -y values. Also paperback books exhibit significantly higher dimension-y values. While hardback books, on the other hand, have intermediate dimension-y value.

# Classification Problems

We have identified three classification tasks:

- The first task involves classifying a book's genre using its title and description, but it is unattainable due to computational resource limitations.
- The second problem seeks to classify a book's rating based on its title, description, and author information. Unfortunately, this classification task is also beyond our reach due to computational constraints.
- The third classification problem entails categorizing a book's format using its dimension-x, dimension-y, dimension-z, and weight.


For the classification problem , we used three different classification algorithms Logistic Regression , Decision tree classifier and Random forest classifier.

- Accuracy of classifiers :
  - Logistic Regression      : 78.12 %
  - Decision Tree            : 88.75 %
  - Random Forest Classifier : 90.03 %

#References :
- Terminlogies and understanding of the dataset : https://www.kaggle.com/datasets/sp1thas/book-depository-dataset
- Model classification and optimization : https://scikit-learn.org/stable/supervised_learning.html
  

# Acknowledgements :
We would like to express our sincere gratitude and appreciation to the Prof. Arpit Rana for his invaluable support and contributions to this project, and that to Vipasha Vaghela, Himanshu Beniwal and Aksh Patel.


