# ML_Project2022_Group20
ML Final Project, Boosting For Fairness-aware Classification, Skoltech 2022
# Datasets
Four datasets were used: [Adult Income Dataset](https://www.kaggle.com/datasets/uciml/adult-census-income), [Bank Dataset](https://www.kaggle.com/datasets/prakharrathi25/banking-dataset-marketing-targets?select=train.csv), [COMPAS dataset](https://raw.githubusercontent.com/propublica/compas-analysis/master/compas-scores-two-years.csv), [KDD Census income dataset](https://archive.ics.uci.edu/ml/datasets/Census-Income+(KDD)).
# Requirement
There are no any requirement for others installation.
# Structure
We Implement Adafair Algorithm proposed by [(Iosifidis & Ntoutsi, 2019)](https://arxiv.org/pdf/1909.08982.pdf)
and another algorithm, SMOTEBooste propsed by [(Chawla et al., 2003)](https://link.springer.com/chapter/10.1007/978-3-540-39804-2_12)
# Results & Presentaion

[Link For Presentation Slide](https://drive.google.com/file/d/1r2A46jfGtDvJcPXSSPWWJNx5mHH_iZ0S/view?usp=sharing)

![Adult](https://user-images.githubusercontent.com/98969542/159535195-86945fe5-abc7-4c04-a384-44a8e7703874.png)


Figure 1 shows the performance of different approaches we tested on the dataset. AdaFair and SMOTEBoost outperform AdaBoost in terms of balance accuracy, with SMOTEBoost achieving the highest accuracy score. Despite the fact that the accuracy and equalized odds of two fairness-aware approaches are lower than AdaBoost, the TPR of both protected and non-protected classes is significantly higher. TNR protected classes of AdaBoost are slightly more than fairness methods in protected classes but significantly more in non-protected classes. Referring to the figure, both fairness-aware approaches can approve the balance accuracy and TPR of protected and non-protected classes of this dataset.

![Bank](https://user-images.githubusercontent.com/98969542/159535215-9707154a-260a-4391-a3a4-d6e110955718.png)


As shown in Figure 2, both fairness-aware approaches perform nearly as well as AdaBoost in terms of accuracy and TNR of both protected and non-protected classes. Furthermore, both techniques outperform AdaBoost in terms of balance accuracy and TPR while falling short in terms of TNR. According to the figure, both fairness-aware approaches can preserve accuracy and TNR while approving the dataset's balance accuracy and TPR.

![Compas](https://user-images.githubusercontent.com/98969542/159535235-64a0f2a9-d7b9-4dbf-8c9a-700b2ac0ad5f.png)


Figure 3 shows that all approaches perform nearly identically in this dataset, with AdaFair scoring slightly higher than the others in almost all cases. According to the figure, both fairness-aware approaches can be utilize to detect the unfair classification in the sensitive attribute.

![KDD](https://user-images.githubusercontent.com/98969542/159535261-905588bb-ff75-4acb-8c7d-a7051943caa0.png)


KDD dataset. As shown in Figure 4, AdaFair has the highest balance accuracy and TPR scores in this dataset, whereas AdaBoost and SMOTEBoost have better accuracy and TNR scores. In equalized odds, SMOTEBoost has the best score. According to the graph, both fairness-aware approaches can be utilized to achieve classification fairness, with AdaFair outperforming the others in TPR.
