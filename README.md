# Supervised Learning Credit Risk Classification

## Overview

### Part One - Logistic Regression Model with Resampling Techniques Evaluation

Part one  evaluates the performance of machine learning, credit risk classification models based on the logistic regression machine learning model paired with with various resampling methods. 

A logistic regression machine learning model is created with each of the following resampling methods

* Random Oversampling
* SMOTE Oversampling
* ClusterCentroids Undersampling
* SMOTEENN

Model performance statistic are generated for each model and resampling method combination.

The performance statistics for all model pairs are analyzed and compared to determine the best performing model and resampling method combination for classifying credit risk.

### Part Two - Ensemble Learning Models Evaluation

Part two evaluates the performance of machine learning, credit risk classification models based on ensemble machine learning models.

Two ensemble machine learning models are created 

* Balanced Random Forest
* AdaBoost

Model performance statistic are generated for each ensemble model.

The performance statistics for the two ensemble machine learning models are compared to the performance statistics of the selected logistic regression sampling model from part one to determine if any of the ensemble learning models perform better at credit risk classification than the model chosen in part one.

## Logistic Regression Resampling Technique Models

### Model Performance Statistics

#### Model Target Resampled Count
<table>
  <thead style="background-color: black">
    <tr>
      <th>Target Category</th>
      <th>Random Over Sampling</th>
      <th>SMOTE Over Sampling</th>
      <th>ClusterCentroids Under Sampling</th>
      <th>SMOTEENN</th>
    </tr>
  </thead
  <tbody>
    <tr>
      <td>Low Risk</td>
      <td>51352</td>
      <td>51352</td>
      <td>260</td>
      <td>62022</td>
     </tr>
    <tr>
      <td>High Risk</td>
      <td>51352</td>
      <td>51352</td>
      <td>260</td>
      <td>68458</td>
     </tr>
  </tbody>
</table>

#### Balanced Accuracy Scores
<table>
  <thead>
    <tr>
      <th>Random Over Sampling</th>
      <th>SMOTE Over Sampling</th>
      <th>ClusterCentroids Under Sampling</th>
      <th>SMOTEENN</th>
    </tr>
  </thead
  <tbody>
    <tr>
      <td>0.7856360112968401</td>
      <td>0.7966770207605626</td>
      <td>0.7752245065690078</td>
      <td>0.5926399313487315</td>
   </tr>
  </tbody>
</table>

#### Confusion Matrices 
<table>
  <thead>
    <tr>
      <th>Sampling Type</th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thead
  <tbody>
    <tr>
      <td>Random Over Sampling</td>
      <td></th>
      <td></th>
    </tr>
    <tr>
       <td>Actually High Risk</td>
       <td>62</td>
       <td>25</td>
    </tr>
    <tr>
      <td>Actually Low Risk</td>
      <td>2420</td>
      <td>14698</td>
    </tr>
    <tr>
      <td></th>
      <td></th>
      <td></th>
    </tr>
    <tr>
      <td>SMOTE Over Sampling</th>
      <td></th>
      <td></th>
    </tr>
    <tr>
       <td>Actually High Risk</td>
       <td>62</td>
       <td>25</td>
    </tr>
    <tr>
      <td>Actually Low Risk</td>
      <td>2042</td>
      <td>15076</td>
    </tr>
    <tr>
      <td></th>
      <td></th>
      <td></th>
    </tr>
    <tr>
      <td>Cluster Centroids Under Sampling</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
       <td>Actually High Risk</td>
       <td>68</td>
       <td>19</td>
    </tr>
    <tr>
      <td>Actually Low Risk</td>
      <td>3957</td>
      <td>13161</td>
    </tr>
    <tr>
      <td></th>
      <td></th>
      <td></th>
    </tr>
    <tr>
      <td>SMOTEENN</td>
      <td>Predicted High Risk</td>
      <td>Predicted Low Risk</td>
    </tr>
    <tr>
       <td>Actually High Risk</td>
       <td>72</td>
       <td>15</td>
    </tr>
    <tr>
      <td>Actually Low Risk</td>
      <td>10995</td>
      <td>6123</td>
    </tr>
  </tbody>
</table>




#### Imbalanced Classification Reports
<table>
  <thead>
    <tr>
      <th>Sampling Type</th>
      <th>Precision</th>
      <th>Recall</th>
      <th>Specificity</th>
      <th>f1</th>
      <th>Geometric Mean</th>
      <th>Index Balanced Accuracy</th>
      <th>Count</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>Random Over Sampling</td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
    </tr>
    <tr>
       <td>High Risk</td>
       <td>0.02</td>
       <td>0.71</td>
       <td>0.86</td>
       <td>0.05</td>
       <td>0.78</td>
       <td>0.60</td>
       <td>87</td>
    </tr>
    <tr>
       <td>Low Risk </td>
       <td>1.00</td>
       <td>0.86</td>
       <td>0.71</td>
       <td>0.92</td>
       <td>0.78</td>
       <td>0.62</td>
       <td>17118</td>
    </tr>
    <tr>
       <td>Avg/Total</td>
       <td>0.99</td>
       <td>0.86</td>
       <td>0.71</td>
       <td>0.92</td>
       <td>0.78</td>
       <td>0.62</td>
       <td>17205</td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
   <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>SMOTE Over Sampling</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>High Risk</td>
      <td>0.03</td>
      <td>0.71</td>
      <td>0.88</td>
      <td>0.06</td>
      <td>0.79</td>
      <td>0.62</td>
      <td>87</td>
    </tr>
    <tr>
      <td>Low Risk</td>
      <td>1.00</td>
      <td>0.88</td>
      <td>0.71</td>
      <td>0.94</td>
      <td>0.79</td>
      <td>0.64</td>
      <td>17118</td>
    </tr>
    <tr>
      <td>Avg/Total</td>
      <td>0.99</td>
      <td>0.88</td>
      <td>0.71</td>
      <td>0.93</td>
      <td>0.79</td>
      <td>0.64</td>
      <td>17205</td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>ClusterCentroids Under Sampling</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
       <td>High Risk</td>
       <td>0.02</td>
       <td>0.78</td>
       <td>0.77</td>
       <td>0.03</td>
       <td>0.78</td>
       <td>0.60</td>
       <td>87</td>
    </tr>
    <tr>
       <td>Low Risk</td>
       <td>1.00</td>
       <td>0.77</td>
       <td>0.78</td>
       <td>0.87</td>
       <td>0.78</td>
       <td>0.60</td>
       <td>17118</td>
    </tr>
    <tr>
       <td>Avg/Total</td>
       <td>0.99</td>
       <td>0.77</td>
       <td>0.78</td>
       <td>0.86</td>
       <td>0.78</td>
       <td>0.60</td>
       <td>17205</td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>SMOTEENN</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
       <td>High Risk</td>
       <td>0.01</td>
       <td>0.83</td>
       <td>0.36</td>
       <td>0.01</td>
       <td>0.54</td>
       <td>0.31</td>
       <td>87</td>
    </tr>
    <tr>
       <td>Low Risk</td>
       <td>1.00</td>
       <td>0.36</td>
       <td>0.83</td>
       <td>0.53</td>
       <td>0.54</td>
       <td>0.28</td>
       <td>17118</td>
    </tr>
    <tr>
       <td>Avg/Total</td>
       <td>0.99</td>
       <td>0.36</td>
       <td>0.83</td>
       <td>0.52</td>
       <td>0.54</td>
       <td>0.28</td>
       <td>17205</td>
    </tr>
  </tbody>
</table>

### Analysis

#### Overview

Financial institutions make most of their profits providing loans to low-credit-risk borrowers. This is because low-credit-risk borrowers are the largest segment of the credit market and have the lowest average loan default rate. High-credit-risk borrowers are much smaller segment of the credit market because they either cannot qualify for a loan or can only obtain a loan with much higher interest rates. Therefore, financial institutions must maximize the number of loans that they issue to low-credit-risk borrowers in order to maximize their profits.


To maximize the number of low-credit-risk loans issued, the highest priority goal of the credit risk classification process must be to accurately classify low-credit-risk borrowers. If the credit risk classification processes misclassifies a significant number of low-credit-risk borrowers as high-credit-risk (false negatives), loans will mistakenly not be issued to a significant number of low-credit-risk borrowers and financial institutions will not realize the profits that these loans would have generated if issued. Therefore, any machine learning model implemented as part of the credit classification process must have a high precision in classifying low-credit-risk borrowers.


The secondary goal of the credit risk classification process must be to minimize the number of high-credit-risk borrowers that are misclassified as low-credit-risk . In the source credit data set, only 0.5% of the borrowers were a high-credit-risk. Therefore, if a financial institution were to misclassify all the high-credit-risk borrowers as a low-credit-risk (false positives), only 0.5% of the loans issued would be to unqualified borrowers. However, the source data only contains credit information for 17,205 borrowers. This source credit data set is too small of a sample to accurately represents the distribution of high and low credit risk borrows of the whole credit market. Data on loan default rates from the Federal Reserve Bank of St. Louis show that [the overall loan default rates ranges from 1.5 to 7.5 5](https://fred.stlouisfed.org/series/DRALACBN) depending on economic conditions at the time of these defaults. If a financial institution were to misclassify 7% of high-credit-risk borrowers as a low-credit-risk and the loans erroneously issued to these borrowers were to be defaulted on, the profits of these financial institutions would be significantly reduced. Therefore, any machine learning model implemented as part of the credit classification process must have a high recall in classifying low-credit-risk borrowers.


The third goal of the credit risk classification process must be to minimize losses from loan defaults. To do this, finanical institution needs to minimize the amount of loans given to high credit-risk borrowers. If a borrower is an actual high credit-risk, then financial institution must accurate classify the borrower as a high-credit-risk. Since high-credit-risk borrowers are a small part of the credit market, financial institution are willing to have a slightly higher number of low-credit-risk borrowers misclassified as high-credit-risk (false positives), in order to insure a high probability of classifying actual high-credit-risk borrowers as high-credit-risk. This is because the total number of borrows classified as high credit-risk overall will be small, even when including the number of low-credit-risk borrowers misclassified as high-credit-risk. The credit risk classification process could include a step that further reviews all borrowers classified as high-credit-risk in order to correct the misclassification of low-credit-risk borrowers as high-credit-risk. Any machine learning model implemented as part of the credit classification process must have a high recall in predicting high-credit-risk borrowers. In addition, the credit classification process can tolerate a machine learning model with a moderately lower precision of misclassifying low-credit-risk borrowers as high-credit-risk (false positives) in order to have a higher recall in classifying actual high-credit-risk borrowers.



In summary to achieve these two goals of

* Maximizing the number of loans made to low-credit-risk borrowers 
* Insuring that actual high credit-risk borrowers are predicted as high credit-risk

the financial institution must implement a machine learning model that

* Classifies low-credit-risk borrowers with high precision and a high recall
* Classifies high-credit-risk borrowers with a high recall
  * Can tolerate lower precision in classifying high-credit-risk borrowers with higher recall



In summary to achieve these two goals of

* Maximizing the number of loans made to low-credit-risk borrowers 
* Insuring that actual high credit-risk borrowers are predicted as high credit-risk

the financial institution must implement a machine learning model that

* Classifies low-credit-risk borrowers with the highest precision and the highest recall
* Classifies high-credit-risk borrowers with the highest recall
  * Can tolerate lower precision in classifying high-credit-risk borrowers in order to classify them with higher recall



#### Model Peformance Comparison

All the machine learning models predict low-credit-risk borrowers with a precision of 1. Therefore, the two machine learning models with the lowest sensitivity in predicting low-credit-risk borrowers

* Logistic regression with cluster centroids resampling
* logistic regression with SMOTEENN resampling

can be eliminated. 

The two remaining models

* Logistic regression with random resampling
* Logistic regression with SMOTE resampling

have the same sensitivity in predicting high-credit-risk borrowers. However, SMOTE resampling has slightly higher precision in predicting high-credit-risk borrows which will reduce the number of low-credit-risk borrows misclassified has high-credit-risk (false positives). Due to this higher precision, the logistic regression with SMOTE resampling would have the highest number of actual low-credit-risk borrowers classified as low-credit-risk. The financial instructions using this machine learning model will issue the maximum number of loans to low-credit-risk borrowers and will maximize profits due the fact that they will be issuing the maximum number of loans to these borrowers. In addition, the balance accuracy score for the logistic regression with SMOTE resampling model is slightly better than balance accuracy score for the logistic regression with random resampling model. Therefore, performance data analysis shows that the logistic regression with SMOTE resampling model would be the best performing machine learning model for credit risk classification.

Another issue to consider is the number of low-credit-risk borrowers that the model misclassifies as high credit-risk borrowers. From the imbalance classification report, the credit risk data set has only 87 actual high-credit-risk borrowers while there are 17118 actual low-credit-risk borrowers. The high-credit-risk borrowers are only 0.5% of the total data set. The logistic regression with SMOTE resampling model incorrectly classifies 2042 low credit-risk borrowers as high-credit-risk. This is 23 time the number of actual high-credit-risk borrower in the data set. In addition, if the financial institution relies solely on a machine learning model for credit classification, the institution will issue 14% less loans to their target low-credit-risk borrowers which in turn will significantly reduce their market share and there profits from this credit market segment. Any financial institution that implements this machine learning model in its current state would have to have a secondary process to further investigate the credit background of the borrowers classifies as high-credit-risk. The institutions cannot afford mistakenly not issue loan to 14% of the low-credit-risk borrowers because the model erroneously classifies the as high-credit-risk.

The final metrics to consider when financial institutions are deciding to implement a credit classification, machine learning model is cost savings, costs, and profits. Institution will realize a cost saving from using a machine learning model to classify the credit risk. This cost saving will come from the reduction in staff needed in the credit risk department due to implementing a machine learning centric, credit risk classification process. In addition, using a machine learning in credit risk classification process will increasing the number of loans made to low-credit-risk borrowers due to a efficiency gains from using a machine learning model in the credit risk classification process. This increase in loan generation to low-credit-risk borrows will increase the profits realize by these financial institutions. 

There are several costs that would be incurred by financial institutions when implementing a machine learning centric, credit risk classification process. These costs include creating a secondary review process to further screen borrowers classified as high-credit-risk by machine learning model correctly. In addition, the institution would incur losses from issuing loans to high-risk-credit borrowers that are misclassified as low-credit-risk borrowers. Finally, the institution would incur the cost of developing a the machine learning centric, credit risk classification process which includes the cost of hiring data scientists and IT staff to develop this process and the cost of upgrading its existing IT infrastructure. 

If the cost saving and increased profits that are realized from implementing a machine learning centric, credit risk process is greater than the cost of implementing this process, the financial institution should implement a machine learning, centric credit risk classification process.


#### Conclusion

This analysis based on a small sample of credit risk data has determined that the logistic regression with SMOTE resampling machine learning model is the best and most valid model that can be used in a credit risk classification process. In addition, it seems likely that the yearly cost saving from the reduction credit risk staff needed for credit risk classification for financial institutions that transitions to a machine learning centric, credit risk process and the increase profits that would be generated the increase in the number of loans made to low-credit-risk clients due to machine learning efficiency will exceed the costs of implementing this process for most financial institutions. Therefore, these institutions consider using this machine learning model for a machine learning centric, credit risk classification process.


## Ensemble Learning Models

### Model Performance Statistics

#### Target

<table>
  <thead>
    <tr>
      <th>Target Category</th>
      <th>Balanced Random Forest Classifier</th>
    </tr>
  </thead
  <tbody>
    <tr>
      <td>Low Risk</td>
      <td>51352</td>
     </tr>
    <tr>
      <td>High Risk</td>
      <td>51352</td>
     </tr>
  </tbody>
</table>


#### Balanced Accuracy Score
<table>
  <thead>
    <th>Balanced Random Forest Classifier</th>
    <th>AdaBoost</th>
  </thead>
  <tbody>
    <tr>
        <td>0.8172844877946586</td>
        <td>0.6264367816091954</td>
   </tr>
  </tbody>
</table>

#### Confusion Matrix
<table>
  <thead>
    <tr>
      <th>Sampling Type</th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thea<
  <tbody>
    <tr>
      <td>Balanced Random Forest Classifier</td>
      <td></th>
      <td></th>
    </tr>
    <tr>
       <td>Actually High Risk</td>
       <td>64</td>
       <td>23</td>
    </tr>
    <tr>
      <td>Actually Low Risk</td>
      <td>1730</td>
      <td>15388</td>
    </tr>
    <tr>
      <td></th>
      <td></th>
      <td></th>
    </tr>
    <tr>
      <td>AdaBoost</th>
      <td></th>
      <td></th>
    </tr>
    <tr>
       <td>Actually High Risk</td>
       <td>22</td>
       <td>65</td>
    </tr>
    <tr>
      <td>Actually Low Risk</td>
      <td>0</td>
      <td>17118</td>
    </tr>
  </tbody>
</table>

#### Imbalanced Classification Report
<table>
  <thead>
    <tr>
      <th> Ensemble Model</th>
      <th>Precision</th>
      <th>Recall</th>
      <th>Specificity</th>
      <th>f1</th>
      <th>Geometric Mean</th>
      <th>Index Balanced Accuracy</th>
      <th>Count</th>
    </tr>
  </thead
  <tbody>
    <tr>
      <td>Balanced Random Forest Classifier</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
       <td>High Risk</td>
       <td>0.04</td>
       <td>0.74</td>
       <td>0.90</td>
       <td>0.07</td>
       <td>0.81</td>
       <td>0.65</td>
       <td>87</td>
    </tr>
    <tr>
       <td>Low Risk</td>
       <td>1.00</td>
       <td>0.90</td>
       <td>0.74</td>
       <td>0.95</td>
       <td>0.81</td>
       <td>0.67</td>
       <td>17118</td>
    </tr>
    <tr>
       <td>Avg/Total</td>
       <td>0.99</td>
       <td>0.90</td>
       <td>0.74</td>
       <td>0.94</td>
       <td>0.81</td>
       <td>0.67</td>
       <td>17205</td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>AdaBoosting</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
       <td>High Risk</td>
       <td>1.00</td>
       <td>0.25</td>
       <td>1.00</td>
       <td>0.40</td>
       <td>0.50</td>
       <td>0.23</td>
       <td>87</td>
    </tr>
    <tr>
       <td>Low Risk</td>
       <td>1.00</td>
       <td>1.00</td>
       <td>0.25</td>
       <td>1.00</td>
       <td>0.50</td>
       <td>0.27</td>
       <td>17118</td>
    </tr>
    <tr>
       <td>Avg/Total</td>
       <td>1.00</td>
       <td>1.00</td>
       <td>0.26</td>
       <td>1.00</td>
       <td>0.50</td>
       <td>0.27</td>
       <td>17205</td>
    </tr>
  </tbody>
</table>

### Analysis

The previous analysis determined that the machine learning model that will perform the best in analyzing credit risk would be a model that

* Classifies low-credit-risk borrowers with the highest precision and the highest recall
* Classifies high-credit-risk borrowers with the highest recall
  * Can tolerate lower precision in classifying high-credit-risk borrowers in order to classify them with higher recall
  
Both the ensemble random forest model and AdaBoost model have higher precision and higher recall in classifying low credit-risk borrowers than the logistic regression model with SMOTE resampling. However, the AdaBoost model has a much lower recall in classifying high-credit-risk borrowers the logistic regression model. Alternatively, the Random Forest model has a higher recall in predicting high-credit-risk borrowers. 

#### Conclusion

The Random Forest model performance statistics indicates that it should have higher performance in classifying credit risk than the logistic regression model with SMOTE resampling model. There should be further testing of these two machine learning model candidates using larger credit risk training sets to determine the consistency of each model’s performance before making the a final decision on what model if any to use.

