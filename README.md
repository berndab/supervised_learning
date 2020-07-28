# Supervised Learning Credit Risk Classification

## Overview

### Logistic Regression Model with Resampling Techniques Evaluation

Part 1 of this project evaluates the performance of machine learning, credit risk classification models based on the logistic regression machine learning model paired with with various resampling techniques 

A logistic regression machine learning model is created with each of the following resampling techniques

* Random Oversampling
* SMOTE Oversampling
* ClusterCentroids Undersampling
* SMOTEENN

Model performance statistic for each model sampling pair combination is generated 
The performance statistics are analyzed to determine the best performing model resampling pair for classifying credit risk

### Ensemble Learning Model Evaluation

Part two of this project evaluates the performance of machine learning, credit risk classification models based on the ensemble learning models

Two ensemble machine learning models are created 

* Balanced Random Forest
* AdaBoost

Model performance statistic for each ensemble machine learning model is generated 
The performance statistics are for these models are compared to the performance statistics for the best performing logistic regression resampling technique model to determine if any of the ensemble learning models perform better then the best performing logistic regression resampling model



## Credit Risk Classification Model Peformance StatisticsPart 1 of this project evaluates the performance of machine learning, credit risk classification models based on the logistic regression machine learning model paired with with various resampling techniques 

A logistic regression machine learning model is created with each of the following resampling techniques

* Random Oversampling
* SMOTE Oversampling
* ClusterCentroids Undersampling
* SMOTEENN

Model performance statistic for each model sampling pair combination is generated 
The performance statistics are analyzed to determine the best performing model resampling pair for classifying credit risk

### Ensemble Learning Model Evaluation

Part two of this project evaluates the performance of machine learning, credit risk classification models based on the ensemble learning models

Two ensemble machine learning models are created 

* Balanced Random Forest
* AdaBoost

Model performance statistic for each ensemble machine learning model is generated 
The performance statistics are for these models are compared to the performance statistics for the best performing logistic regression resampling technique model to determine if any of the ensemble learning models perform better then the best performing logistic regression resampling model

### Logistic Regression Resampling Technique Models

#### Model Target Resampled Count
<table>
  <thead>
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
      <th>Random Over Sampling</th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thead
  <tbody>
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
  </tbody>
</table>


<table>
  <thead>
    <tr>
      <th>SMOTE Over Sampling</th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thead
  <tbody>
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
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>ClusterCentroids Under Sampling</th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thead
  <tbody>
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
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>SMOTEENN</th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thead
  <tbody>
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
      <th>Random Over Sampling</th>
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
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>SMOTE Over Sampling</th>
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
      <td>Low Risk </td>
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
  </tbody>
</table>

<table>
  <thead>
     <tr>
      <th>ClusterCentroids Under Sampling</th>
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
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>SMOTEENN</th>
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

Financial institutions make the majority of their profits providing loans to low-credit-risk borrowers. This is because low-credit-risk borrowers are the largest market segment of the credit market. High credit-risk borrowers are much smaller segment of the credit market because they are only able to obtain loans with much higher interest rates. Therefore, fewer of these borrowers have the financial resources to pay a higher interest rate for a loan. In order for a financial institution to maximize their share of the low-credit-risk segment of the credit market and maximize profits from this market segment, financial institution need to maximize the number of loans made to low-credit-risk borrows. To do this, they must minimize misclassifying high credit-risk borrowers as low-credit-risk borrowers and minimize misclassifying low-credit-risk borrowers as high-credit-risk borrowers. 

In addition, financial institutions want to minimize losses from load defaults. To do this. these institution needs to minimize the amount of loans given to high credit-risk borrowers. Therefore, if a potential borrower is a high credit-risk, the financial institution wants to avoid misclassifying the borrower as a low-credit-risk. Since high-credit-risk borrowers are a small part of the credit market, financial institution are willing to have a high number of low-credit-risk borrowers misclassified as high credit-risk borrows in order to insure a high probability classifying actual high-credit-risk borrowers as high-credit-risk. This is because the total number of borrow classified as high credit-risk borrowers overall will be small even including misclassified low-credit-risk borrows. 

To achieve these two goals of
*Maximizing the number of loans made to low-credit-risk borrowers
*Insuring that actual high credit-risk borrowers are predicted as high credit-risk borrowers

the financial institution must choose a machine learning model that 

* Predicts low-credit-risk borrowers with high precision and a high recall 
* Predicts high-credit-risk borrowers with a high recall

Looking at the candidate machine learning models for predicting credit risk, all of them predict low-credit-risk borrowers with a precision of 1. Therefore, the two machine learning models with the lowest sensitivity in predicting low-credit-risk borrowers, logistic regression with cluster centroids resampling and logistic regression with SMOTEENN resampling, can be eliminated. 

The two remaining models, logistic regression with random resampling and logistic regression with SMOTE resampling, have the same sensitivity in predicting high-credit-risk borrowers. However SMOTE resampling has slightly higher precision in predicting high-credit-risk borrows which will reduce the number of low-credit-risk borrows misclassified has high-credit-risk. Therefore, the logistic regression with SMOTE resampling would have the highest number of actual low-credit-risk borrowers predicted as low-credit-risk borrowers. Financial instruction using this machine learning model will make the issue the maximum number of loans to low-credit-risk borrowers and will therefore maximize profits. Therefore, the logistic regression with SMOTE resampling would be the best machine learning model financial institutions should use for credit risk prediction. This determination is further confirm by the fact that the balance accuracy score for logistic regression with SMOTE resampling model is slightly better than balance accuracy score for the logistic regression with random resampling model.

The final issue to consider is the number of low-credit-risk borrowers that the model misclassifies as high credit-risk borrowers. From the imbalance classification report, the credit risk data set has only 87 actual high-credit-risk borrowers while there are 17118 actual low-credit-risk borrowers. The high-credit-risk borrowers are only 0.5% of the total data set. The logistic regression with SMOTE resampling model incorrectly classifies 2042 low credit-risk borrowers as high-credit-risk. This is 23 time the number of actual high-credit-risk borrower in the data set. In addition, if the financial institution relies solely on the machine learning model’s credit predictions, the institution will issue 14% less loans to low-credit-risk borrowers which will significantly reduce its market share and profits from this credit market segment. 
Any financial institution that implements this machine learning model in its current state would have to have a secondary process to further investigate the credit background of the borrowers that that model classifies as high-credit-risk. The institutions cannot afford to fail to make loans to 14% of the low-credit-risk borrowers because the model falsely classifies the as high-credit-risk.

Thus, final metric that will determine if implementing a credit classification machine learning model will benefit a financial institution is cost savings. Institution will realize a cost saving from using a machine learning model to classify the credit risk. This cost saving will come from the reduction in staff needed in the credit risk department that used a machine learning centric credit risk classification process.  

However, the institution would have to incur the cost of creating a secondary review process to further screen borrowers who are classified as high-credit-risk by the model.  In addition, the institution would incur losses from giving loans to high-risk-credit borrowers that the machine learning model misclassified as low-credit-risk borrowers. Finally, the institution would incur the cost of developing a the machine learning centric credit risk classification process, the cost of hiring data scientists and IT staff, and the potential cost have to upgrade its existing IT infrastructure.

If the cost saving from implementing a machine learning model centric credit risk process is greater than the cost of implementing this process, the financial institution should implement machine learning centric process. 

#### Conclusion

This limited analysis has concluded that the logistic regression with SMOTE resampling machine learning model is the best and most valid model that financial institution should use in for credit risk classification. In addition, it seems likely that the yearly cost saving from the reduction credit risk staff needed in financial institutions that use this machine learning model will exceed the costs of implementing this model for most institutions. Therefore, these institutions should further investigate this model as a candidate model for a machine learning centric credit risk classification process.



### Ensemble Learning Models

### Balanced Random Forest Classifier

#### Target
<table>
  <thead>
    <tr>
      <th>Target Category</th>
      <th>Count</th>
    </tr>
  </thead
  <tbody>
    <tr>
      <td>Low Risk</td>
      <td>68470</td>
    </tr>
    <tr>
      <td>High Risk</td>
      <td>347</td>
    </tr>
  </tbody>
</table>

#### Balanced Accuracy Score
<table>
  <tbody>
    <tr>
        <td>0.8172844877946586</td>
    </tr>
  </tbody>
</table>

#### Confusion Matrix
<table>
  <thead>
    <tr>
      <th></th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thead
  <tbody>
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
  </tbody>
</table>

#### Imbalanced Classification Report
<table>
  <thead>
    <tr>
      <th></th>
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
  </tbody>
</table>


### AdaBoosting


#### Balanced Accuracy Score
<table>
  <tbody>
    <tr>
        <td>0.6264367816091954</td>
    </tr>
  </tbody>
</table>

#### Confusion Matrix
<table>
  <thead>
    <tr>
      <th></th>
      <th>Predicted High Risk</th>
      <th>Predicted Low Risk</th>
    </tr>
  </thead
  <tbody>
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
      <th></th>
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

In the analysis above it was determined that the machine learning model that will perform the best in analyzing credit risk would be a model that

* Predicts low-credit-risk borrowers with high precision and a high recall 
* Predicts high-credit-risk borrowers with a high recall


Both the ensemble random forest model and AdaBoost model have higher precision and higher recall in classifying low credit-risk borrows than the logistic regression model with SMOTE resampling. However the AdaBosst model has a much lower recall in prediction high-credit-risk borrowers while Random Forest has a higher recall in predicting high-credit-risk borrower. 

#### Conclusion

The performance data for the Random Forest model indicates that is should be a better model for classifying credit risk than the logistic regression model with SMOTE resampling model.
