                                                                𝐖𝐞𝐛 𝐒𝐜𝐫𝐚𝐩𝐢𝐧𝐠, 𝐃𝐚𝐭𝐚 𝐂𝐥𝐞𝐚𝐧𝐢𝐧𝐠 𝐚𝐧𝐝 𝐓𝐨𝐩𝐢𝐜 𝐂𝐥𝐚𝐬𝐬𝐢𝐟𝐢𝐜𝐚𝐭𝐢𝐨𝐧 𝐏𝐢𝐩𝐞𝐥𝐢𝐧𝐞:

𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐎𝐯𝐞𝐫𝐯𝐢𝐞𝐰:
This project implements a pipeline to scrape articles by a specific author, clean the data, and classify topics using Natural Language Processing (NLP). The pipeline processes articles for a well-organized dataset structured around key themes.

𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬--->

Web Scraping: Extracts articles written by a specific author across multiple pages, handling pagination and dynamic loading.

Data Cleaning: Processes and cleans text to remove irrelevant content, normalize formatting, and standardize metadata.

Topic Classification: Categorizes articles into predefined topics, utilizing NLP techniques for accurate classification.


𝐑𝐞𝐪𝐮𝐢𝐫𝐞𝐦𝐞𝐧𝐭𝐬:

Programming Language: Python 


𝐋𝐢𝐛𝐫𝐚𝐫𝐢𝐞𝐬:

requests, BeautifulSoup4: For web scraping.

pandas: For data manipulation and storage.

sklearn (scikit-learn): For NLP-based topic classification.

nltk or spaCy: For text preprocessing.


𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐒𝐭𝐫𝐮𝐜𝐭𝐮𝐫𝐞:


├── Scrapping.py           # Web scraping script for article extraction

├── data_cleaning.py     # Data cleaning functions

├── topic_classification.py # NLP-based topic classification code

├── articles.csv         # Output dataset with cleaned and categorized articles

├── README.md            # Project documentation

└── requirements.txt     # Required libraries

𝐔𝐬𝐚𝐠𝐞:

1. Web Scraping
The Scrapping.py script collects all articles for a particular author across multiple pages of a specified website. I have used BeautifulSoup to navigate and extract content.


2. Data Cleaning
The data_cleaning.py script removes unnecessary content like ads, extraneous HTML tags, comments, and irrelevant text from the scraped articles. I have also normalized the text (i.e., 𝐥𝐨𝐰𝐞𝐫𝐜𝐚𝐬𝐞 𝐜𝐨𝐧𝐯𝐞𝐫𝐬𝐢𝐨𝐧, 𝐩𝐮𝐧𝐜𝐭𝐮𝐚𝐭𝐢𝐨𝐧 𝐫𝐞𝐦𝐨𝐯𝐚𝐥).In the end, we have printed out the fields like: 𝐓𝐢𝐭𝐥𝐞, 𝐂𝐨𝐧𝐭𝐞𝐧𝐭, 𝐚𝐧𝐝 𝐃𝐚𝐭𝐞.

3. Topic Classification
The topic_classification.py script uses NLP techniques to categorize each article. CountVectorizer is used for feature extraction, and Naive Bayes, SVM used for topic classification. Applies classification algorithms (e.g., Naive Bayes, SVM) for supervised learning or LDA for unsupervised topic modeling. Achieves target classification accuracy and outputs a structured dataset.


𝐎𝐮𝐭𝐩𝐮𝐭:

The final dataset (articles.csv) includes:

Title: Title of the article.

Content: Cleaned article content.

Date: Publication date of the article.

Topic: Classified topic label.


𝐊𝐧𝐨𝐰𝐧 𝐋𝐢𝐦𝐢𝐭𝐚𝐭𝐢𝐨𝐧𝐬:

Website Structure Changes: The scraper relies on the website’s current HTML structure, which may change.

Model Accuracy: Topic classification model accuracy may vary based on training data volume and quality.
