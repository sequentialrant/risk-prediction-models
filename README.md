# Risk Prediction Models in Healthcare
This repo lists resources for understanding and building risk prediction models in healthcare, especially involving time-to-event data, also called survival analysis. There is a huge volume of scientific literature, and books published on this topic. The intention is to list those that are accessible. To a certain extent, I shall also list resources that includes modeling data involving repeated measurements (longitudinal analysis).

# Books
* [Survival Analysis: A Self-Learning Text](https://www.amazon.com/Survival-Analysis-Self-Learning-Statistics-Biology/dp/1441966455) - a succintly written book in simple English, for someone who wishes to understand survival analysis conceptually
* [Regression Modeling Strategies: With Applications to Linear Models, Logistic and Ordinal Regression, and Survival Analysis](https://www.amazon.com/Regression-Modeling-Strategies-Applications-Statistics/dp/3319194240/ref=sr_1_1?keywords=regression+modeling+strategies&qid=1659000046&s=books&sprefix=regression+modeling+s%2Cstripbooks%2C329&sr=1-1) - read this book after having a conceptual understanding
* [Medical Risk Prediction Models](https://www.amazon.com/Medical-Risk-Prediction-Models-Biostatistics/dp/113838447X/ref=sr_1_2?crid=BJJIAHB3SDOD&keywords=medical+risk+prediction+models+with+ties+to+machine+learning&qid=1659005057&s=books&sprefix=medical+risk+prediction+models+with+ties+to+machine+learning%2Cstripbooks-intl-ship%2C313&sr=1-2) - this book will teach you to ask the right questions, and prepare you for the analysis of prognostic models

# R and Python Packages
The following are the widely used R and Python libraries.
| R        | Python           |
| ------------- |:-------------:|
| [survival](https://cran.r-project.org/web/packages/survival/index.html)     | [lifelines](https://lifelines.readthedocs.io/en/latest/) |
| [riskRegression](https://cran.r-project.org/web/packages/riskRegression/index.html)      | [scikit-survival](https://scikit-survival.readthedocs.io/en/stable/)      |
| [prodLim](https://cran.r-project.org/web/packages/prodlim/index.html) |       |
| [rfsrc](https://www.rdocumentation.org/packages/randomForestSRC/versions/3.1.0/topics/rfsrc) |   |

# Training Courses
* [Statistical methods for risk prediction and prognostic models](https://www.prognosisresearch.com/training-courses)
* [Survival analysis](https://www.statistics.com/courses/survival-analysis/)
* [AI for medicine specialization](https://www.deeplearning.ai/courses/ai-for-medicine-specialization/)

# Research Papers
* [A Predictive Model for Progression of Chronic Kidney Disease to Kidney Failure](https://jamanetwork.com/journals/jama/fullarticle/897102) - this paper applies survival analysis technique to understand the prognosis of chronic kidney disease. It uses electronic health records (EHRs) of patients with kidney disease to predict their disease progression. The creator of this model has exposed their API freely through web browser - the famous [Kidney Failure Risk Equation (KFRE)](https://kidneyfailurerisk.com/). The model parameters can be obtained through their online supplement
* [Random Survival Forests](https://projecteuclid.org/journals/annals-of-applied-statistics/volume-2/issue-3/Random-survival-forests/10.1214/08-AOAS169.full) - Random forest method applied to time-to-event data. Provides a detailed description of the algorithm
* [WTTE-RNN: Weibull Time To Event Recurrent Neural Network](https://publications.lib.chalmers.se/records/fulltext/253611/253611.pdf) - this paper introduces Recurrent Neural Network (RNN) technique to model time-to-event outcomes in the case of discrete or continuous censored data. There is a Keras implementation of this technique [here](https://github.com/daynebatten/keras-wtte-rnn)
* [Prognosis of chronic kidney disease with normal-range proteinuria: The CKD-ROUTE study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5771558/pdf/pone.0190493.pdf)
* [Lessons learnt when accounting for competing events in the external validation of time-to-event prognostic models](https://academic.oup.com/ije/article/51/2/615/6468864) - this paper discusses the importance of accounting for competing risks when validating the progonostic models externally. This paper has also provided their R codes explaing how to validate a competing-risk model
* [The harm of class imbalance corrections for risk prediction models: illustration and simulation using logistic regression](https://arxiv.org/ftp/arxiv/papers/2202/2202.09101.pdf)
* [Calculating the sample size required for developing a clinical prediction model](https://www.bmj.com/content/368/bmj.m441)
* [Assessing performance and clinical usefulness in prediction models with survival outcomes: practical guidance for Cox proportional hazards models](https://www.medrxiv.org/content/10.1101/2022.03.17.22272411v1)
