# Supervised Learning

## Overview

## Logistic Regression Results Using Different Sampling Techniques


#### Target Resampled
<table>
  <thead>
    <tr>
      <th>Target Category</th>
      <th>Random OverSampler</th>
      <th>SMOTE Oversampler</th>
      <th>ClusterCentroids Undersampler</th>
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

#### Balanced Accuracy Score
<table>
  <thead>
    <tr>
      <th>Random OverSampler</th>
      <th>SMOTE Oversampler</th>
      <th>ClusterCentroids Undersampler</th>
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

#### Confusion Matrix
<table>
  <thead>
    <tr>
      <th>Random OverSampler</th>
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
      <th>SMOTE</th>
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
      <th>ClusterCentroids</th>
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




#### Imbalanced Classification Report
<table>
  <thead>
    <tr>
      <th>Random OverSampler</th>
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
      <th>SMOTE</th>
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
      <th>ClusterCentroids</th>
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

Financial institutions make most of their profits providing loans to low-credit-risk borrowers. This is because low-credit-risk borrowers are the largest market share of the credit market. High credit-risk borrowers are much smaller share of the credit market. This is because they are only able to obtain loans with much higher interest rates. Therefore, fewer of these borrowers have the financial resources to pay a higher interest rate for a loan. In order maximize their share of the low-credit-risk segment of the credit market and maximize profits from this market segment,  financial institution wants to maximize the number of loans made to low-credit-risk borrows. To do this, they must minimized misclassifying high credit-risk borrowers as low-credit-risk borrowers and minimize misclassifying low-credit-risk borrowers as high-credit-risk borrowers. 


In addition, financial institutions want to minimize losses do to load defaults. To do this these institution needs to minimize the amount of loans given to high credit-risk borrowers. Therefore, if a potential borrower is a high credit-risk, the financial institution wants to avoid misclassifying the borrower as a low-credit-risk borrower. Since high-credit-risk borrowers are a small part of the credit market, financial institution are willing to have a high number of low-credit-risk borrowers classified as high credit-risk borrows in order to insure a high number of actual high-credit-risk borrowers are classified accurately. This is because the total number of borrow classified as high credit-risk borrowers overall will be much small even including misclassified low-credit-risk borrows. 


To achieve these two goals of
* Maximizing the number of loans made to low-credit-risk borrowers
* Insuring that actual high credit-risk borrowers are predicted as high credit-risk borrowers
the financial institution must choose a machine learning model that 
* Predicts low-credit-risk borrowers with high precision and a high recall 
* Predicting high credit-risk borrowers with a high sensitivity

Looking at the candidate machine learning models for predicting credit risk. all the them have a predict low-credit-risk borrowers with a precision of 1. Therefore, the two machine learning models with the lowest sensitivity in predicting low-credit-risk borrowers, logistic regression using  cluster centroids resampling and logistic regression using SMOTEENN resampling, can be eliminated. The two remaining models, logistic regression using random resampling and logistic regression using SMOTE, have the same sensitivity in predicting high-credit-risk borrowers. However SMOTE, has slightly higher precision in predicting high-credit-risk borrows which will reduce the number of low-credit-risk borrows classified has high-credit-risk borrower. Therefore, the logistic regression with SMOTE would have the highest number of actual low-credit-risk borrowers predicted as low-credit-risk borrowers. Therefore this model would result it the financial instruction making the maximum number of loads to low-credit-risk borrower and maximize the profits made by the financial institution. Therefore the logistic regression with SMOTE resampling would be the best model to use by financial institutions for credit risk prediction. 




## Ensemble Learning

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
      <th>Pre</th>
      <th>Recall</th>
      <th>Specificity</th>
      <th>f1</th>
      <th>Geometric Mean</th>
      <th>Index Balanced Accuracy</th>
      <th>Sup</th>
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

In the analysis above it was determined that the machine learning model that will perform the best in analyzing credit risk would be a model with high precision classifying low credit-risk borrows and high recall in predicting high credit-risk borrowers. Both the ensemble random forest model and AdaBoost model have lower precision classifying low credit-risk borrows and lower recall in predicting high credit-risk borrowers then the logistic regression models using resampling techniques. Thus, these models would not perform as well for credit risk analysis. Using logistic regression model with the SMOTE resampling technique would still perform best for credit risk analysis.
