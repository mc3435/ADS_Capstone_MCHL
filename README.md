# ADS Capstone - Fall 2024
Fall 2023 Capstone Project 

## Table of Contents
  * [Team Members](#team-members)
  * [Abstract](#abstract)
  * [Visual Abstract](#visual-abstract)
  * [Background](#background)
  * [Problem Statement](#problem-statement)
  * [Data Source](#data-source)
  * [Model Evaluations](#model-evaluations)
  * [Conclusion](#conclusion)
  * [References](#references)
    
## Team Members
- Mackenzie Carter [@mc3435](https://github.com/mc3435)
  
- Harini Lakshmanan [@harinigautham](https://github.com/harinigautham) 

## Abstract
This study investigates the ability to use previous medical records to identify genetic disorder risk in patients. Genodetect, a machine learning solution tailored to meet this objective, is presented with the motivation to address the imperative need for early detection and intervention in genetic disorders, with a focus on real-life integration for practical healthcare applications. GenoDetect’s key objective is to build an adaptable model capable of precisely identifying increased risk for genetic disorders, catering to diverse, or even incomplete, medical records. The study employs the Genomes and Genetics dataset, extracted from Kaggle, and employs Extreme Gradient Boosting (XGBoost) as the successful modeling technique. Despite limitations including dataset quality and imbalance of provided outcomes, results show the efficacy of XGBoost and other models in predicting genetic disorder risks based on medical history, particularly excelling in identifying true positives. However, the study acknowledges the complexity of the genetic landscape and recognizes potential limitations in generalizability to diverse populations. This research offers a comprehensive foundation for advancing genetic disorder prediction, showcasing the practical utility of GeneDetect. The implications of this study lie in the tangible applications of machine learning in healthcare diagnostics, emphasizing the importance of early identification for improved patient outcomes.

## Visual Abstract 
<img width="598" alt="599_vis_abstract" src="https://github.com/mc3435/ADS_Capstone_MCHL/assets/97000763/a876e637-243b-4ca3-8b85-8cbbdb0fdd50">

## Background
Understanding an individual’s genetic predisposition to these disorders requires a comprehensive analysis of their medical history. GenoDetect aims to enhance the process of identifying existing and future genetic disorder risks through machine learning methods. The main purpose of this product is to provide an end-to-end, embeddable service that can assist medical practitioners in identifying patients who may benefit from further genetic testing. Previous studies have explored machine learning for genetic disorder prediction but fail to provide a pathway for real-life integration. 

## Problem Statement
We aim to develop a system that can accurately predict the risk of an individual or their offspring developing a genetic disorder.


## Data Source
This project utilizes the [Of Genomes And Genetics](https://www.kaggle.com/datasets/aryarishabh/of-genomes-and-genetics-hackerearth-ml-challenge/) data set

Number of Variables: 45 Columns

Size of Dataset: 22,083 Rows

## Model Evaluations
<img width="604" alt="image" src="https://github.com/mc3435/ADS_Capstone_MCHL/assets/97000763/72398a31-4ed5-4455-9e36-a4fcf173401b">

<img width="604" alt="599_ROC" src="https://github.com/mc3435/ADS_Capstone_MCHL/assets/97000763/e27155ef-a479-45ac-a166-4b5650d796d3">

## Conclusion
In summary, this study tested a variety of classification models, with extreme gradient boosting successfully predicting genetic disorder risk based on previous medical history. Beyond the most optimal performance metrics, XGBoost offers several other advantages over other algorithms such as processing speed, scalability, flexible hyperparameter tuning for optimal performance, and its ability to handle missing data. Though we handled missing data in this project for other tested models, a model that can handle missing data on its own reduces preprocessing time in future applications. XGBoost’s complexity must be noted, as the interpretability of this model is often challenging, especially as the complexity of the model increases. XGBoost can often be referred to as a “Black Box” model, limiting interpretability for the trade-off of high performance (Rudin, 2019). 
	Previous work on this data focused entirely on prediction of specific disorders within the data set (Raza et al., 2023) or only tested a limited number of machine learning models (Ghazal et al., 2022). Raza and colleagues also determined that XGBoost had the best performance in multi-class prediction, compared to our work in binary classification. Multi-class prediction was explored for this project but recurring errors and the project’s short timeline lead to exclusion from this manuscript. While not as complex as previous discussions, the work done here provides a foundation for generic risk prediction, opening a door for later work for risk prediction in a wide range of disorders, beyond those supplied in the given data set. 

## References
Ghazal, T. M., Al Hamadi, H., Umar Nasir, M., Atta-Ur-Rahman, Gollapalli, M., Zubair, M., Adnan Khan, M., & Yeob Yeun, C. (2022). Supervised machine learning empowered multifactorial genetic inheritance disorder prediction. Computational Intelligence and Neuroscience, 2022, Article 1051388. https://doi.org/10.1155/2022/1051388

Kundu, R. (2022, December 16). F1 score in machine learning: Intro & calculation. V7. https://www.v7labs.com/blog/f1-score-guide 

National Human Genome Research Institute. (2020, August 24). Deoxyribonucleic acid (DNA) fact sheet. https://www.genome.gov/about-genomics/fact-sheets/Deoxyribonucleic-Acid-Fact-Sheet 

Raza, A., Rustam, F., Siddiqui, H. U. R., Diez, I. T., Garcia-Zapirain, B., Lee, E., & Ashraf, I. (2023). Predicting genetic disorder and types of disorder using chain classifier approach. Genes, 14(1), Article 71. https://doi.org/10.3390/genes14010071

Rudin, C. (2019. Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead. Nature Machine Intelligence, 1, 206–215. https://doi.org/10.1038/s42256-019-0048-x

Solomon, D. D., Sonia, Kumar, K., Kushal, K., Iyer, S., & Kumar, M. (2023). Extensive review on the role of machine learning for multifactorial genetic disorders prediction. Archives of Computational Methods in Engineering. https://doi.org/10.1007/s11831-023-09996-9

Zhang, L., Lu, D., Bi, X., Zhao, K., Yu, G., & Quan, N. (2023). Predicting disease genes based on multi-head attention fusion. BMC bioinformatics, 24(1), 162. https://doi.org/10.1186/s12859-023-05285-1

Zhou Z., Liu Y., Feng Y., Klepin S., Tsimring     LS., Pillus L., Hasty J., Hao N. (2023). Engineering longevity-design of a synthetic gene oscillator to slow cellular aging. Science, 380, 376-381. DOI:10.1126/science.add7631






