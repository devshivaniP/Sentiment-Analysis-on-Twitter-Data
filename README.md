# Sentiment Analysis on Twitter Data (Major Project)

![Image](https://pluspng.com/img-png/twitter-logo-png-twitterbird-twitter-png-logo-1528.png)

## Overview

This project focuses on building a sentiment analysis model capable of determining the sentiment of tweets as (positive or negative) of a given piece of text. Sentiment analysis is widely used in various applications, such as customer feedback analysis, social media monitoring, and market research.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Data](#data)
- [Models](#models)
- [Evaluation](#evaluation)
- [Future Scope](#futurescope)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Installation

To run this project, you need to have Python installed. It is recommended to use a virtual environment to manage dependencies. Follow the steps below to set up the project:

1. Clone the repository:

```
git clone https://github.com/devShivaniP/twitter-sentiment-analysis.git
cd twitter-sentiment-analysis
```

2. Create a virtual environment:

```
python -m venv venv
```

3. Activate the virtual environment:

- On Windows:

  ```
  venv\Scripts\activate
  ```

- On macOS/Linux:

  ```
  source venv/bin/activate
  ```

## Prerequisites

- Python 3.7+
- Jupyter Notebook
- Necessary Python packages 

## Data

A dataset of 1600000 tweets in English coming from Kaggle. It contains columns like:

- Target
- Ids
- Date
- Flag
- Tweet or Text

 We are only interested by the Text column corresponding to our Target column taking a binary value;
- 0 if the tweet is negative
- 1 if the tweet is positive

## Data Preprocessing

Data obtained from twitter is not fit for extracting features. Mostly tweets consists of message 
along with usernames, empty spaces, special characters, stop words, emoticons, 
abbreviations, hash tags, time stamps, URL’s ,etc. Thus to make this data fit for mining we 
pre-process this data by using various function of NLTK

- Removed URL (Uniform resource locator)
- Removed RT (Re-Tweet)
- Removed duplicates
- Removed Numbers
- Removed Punctuation
- Removed Stopwords
- Converted text into lowercase
- Tokenize the text

## Model Training

1. Naïve-Bayes Classifier 
2. MultinomialNB Classifier 
3. BernoulliNB Classifier 
4. Logistic Regression Classifier
5. Decision Tree Classifier

## Evaluation

- Precision
- Recall
- f1 score
 
## Future Scope

Some of future scopes that can be included in our research work are:

1. Use of parser can be embedded into system to improve results.

2. We can improve our system that can deal with sentences of multiple meanings.

3. We can also increase the classification categories so that we can get better results.
4. We can start work on multi languages like Hindi, Spanish, and Arabic to provide sentiment analysis to more local.
5. We have not considered neutral tweets in this project, which limited the scope of our project.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments

I would like to thank the contributors and the open-source community for their valuable resources and support. Special thanks to [Kaggle] (https://kaggle.com/) for providing datasets and [Scikit-learn](https://scikit-learn.org/) for the machine learning tools. We are highly indebted to Dr. Swati Verma (Project Guide) and Dr. RAKESH BISHT (Assistant Professor and Project Head) of our college for their guidance and constant supervision as well as for providing necessary information regarding the project & also for their support in completing the project.

## References

1. H. Zang, “The optimality of Naïve-Bayes”, Proc. FLAIRS, 2004
2. C.D. Manning, P. Raghavan and H. Schütze, “Introduction to Information Retrieval”, Cambridge University Press, pp. 234-265, 2008
3. A. McCallum and K. Nigam, “A comparison of event models for Naive Bayes text
classification”, Proc. AAAI/ICML-98 Workshop on Learning for Text Categorization, pp.
41-48, 1998
4. M. Schmidt, N. L. Roux and F. Bach, “Minimizing finite Sums with the Stochastic
Average Gradient”, 2002
5. ‘Y. LeCun, L. Bottou, G. Orr and K. Muller, “Efficient BackProp”, Proc. In Neural
Networks: Tricks of the trade 1998.
6. T. Wu, C. Lin and R. Weng, “Probality estimates for multi-class classification by pairwise
coupling”, Proc. JMLR-5, pp. 975-1005, 2004
7. “Support Vector Machines” [Online],<http://scikitlearn.org/stable/modules/svm.html#svm->
classification, Accessed Jan 2016
8. P. Pang, L. Lee and S. Vaithyanathan, “Thumbs up? sentiment classification using
machine learning techniques”, Proc. ACL-02 conference on Empirical methods in natural
language processing, vol.10, pp. 79-86, 2002
9. P. Pang and L. Lee, “Opinion Mining and Sentiment Analysis. Foundation and Trends in
Information Retrieval”, vol. 2(1-2), pp.1-135, 2008
10. E. Loper and S. Bird, “NLTK: the Natural Language Toolkit”, Proc. ACL-02 Workshop
on Effective tools and methodologies for teaching natural language processing and
computational linguistics ,vol. 1,pp. 63-70, 2002
11. H. Wang, D. Can, F. Bar and S. Narayana, “A system for real-time Twitter sentiment analysis of 2012 U.S.presidential election cycle”, Proc. ACL 2012 System Demostration, pp. 115-120, 2012
12. O. Almatrafi, S. Parack and B. Chavan, “Application of location-based sentiment
analysis using Twitter for identifying trends towards Indian general elections 2014”. Proc.
The 9th International Conference on Ubiquitous Information Management and
Communication,2015
13. L. Jiang, M. Yu, M. Zhou, X. Liu and T. Zhao, “Target-dependent twitter sentiment
classification”, Proc. The 49th Annual Meeting of the Association for Computational
Linguistics: Human Language Technologies, vol. 1, pp. 151-160, 2011
14. C. Tan, L. Lee, J. Tang, L. Jiang, M. Zhou and P. Li, “User-level sentiment analysis
incorporating social networks”, Proc. The 17th ACM SIGKDD international conference on
Knowledge discovery and data mining, pp. 1397-1405, 2011
15. A. Pak and P. Paroubek, “Twitter as a Corpus for Sentiment Analysis and Opinion
Mining”, vol. 10, pp. 1320-1326, 2010
16. B. Sun and TY. V. Ng, “Analyzing Sentimental influence of Posts on Social Networks”,
Proc. The 2014 IEEE 18th International Conference on Computer Supported Cooperative
Work in Design, 2014
17. A. Go, R. Bhayani and L. Huang, “Twitter sentiment classification using distant
supervision”, CS224N Project Report, Stanford, vol.1-12, 2009
18. A. Barhan and A. Shakhomirov, “Methods for Sentiment Analysis of Twitter Messages”,
Proc.12th Conference of FRUCT Association, 2012
19. T. Mitchell, “Machine Learning”, McGraw Hill, 1997
20. F. Jensen, “An Introduction to Bayesian Networks”, Springer, 1996
21. T. C. Peng and C. C. Shih, “An Unsupervised Snippet-based Sentiment Classification Method for Chinese Unknown Phrases without using Reference Word Pairs”.IEEE/WIC/ACM Int. Conf. on Web Intelligence and Intelligent Agent Technology, vol. 3, pp. 243-248, 2010
22. R. Feldman, “Techniques and applications for sentiment analysis”, Proc. ACM, pp. 56-
82, 2009
23. N. Cristianini and J. Shawe-Taylor, “ An Introduction to Support Vector Machines and
Other Kernel-based Learning Methods”, Cambridge University Press, March 2000
