# Supervised Learning

## Overview

## Logistic Regression Results Using Different Sampling Techniques

### Random OverSampler

#### Target Resamplled

##### Resampling Data
<table>
  <thead>
    <tr>
      <th>Target Category</th>
      <th>Count</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>low_risk</td>
       <td>high_risk</td>
    </tr>
    <tr>
      <td>51352</td>
      <td>51352</td>
    </tr>
  </tbody>
</table>
##### Balanced Accuracy Score
<table>
  <tbody>
    <tr>
        <td>0.7856360112968401</td>
    </tr>
  </tbody>
</table>

##### Confusion Matrix
<table>
  <thead>
    <tr>
      <th></th>
      <th>Predicted True</th>
      <th>Predicted False</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>Actual True</td>
       <td>62</td>
       <td>25</td>
    </tr>
    <tr>
      <td>Actual False</td>
      <td>2420</td>
      <td>14698</td>
    </tr>
  </tbody>
</table>

##### Imbalanced Classification Report
<table>
  <thead>
    <tr>
      <th></th>
      <th>pre</th>
      <th>rec</th>
      <th>spe</th>
      <th>f1</th>
      <th>geo</th>
      <th>iba</th>
      <th>sup</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>high_risk</td>                                            
       <td>0.02</td>
       <td>0.71</td>
       <td>0.86</td>
       <td>0.05</td>
       <td>0.78</td>
       <td>0.60 </td>
       <td>87</td>
    </tr>
    <tr>
       <td>low_risk </td>                                         
       <td>1.00</td>                                           
       <td>0.86</td>
       <td>0.71</td>
       <td>0.92</td>
       <td>0.78</td>
       <td>0.62</td>
       <td>17118</td>
    </tr>
    <tr>
       <td>avg / total</td>                                         
       <td>0.99</td>                                           
       <td>0.86</td>
       <td>0.71 </td>
       <td>0.92</td>
       <td>0.78</td>
       <td>0.62</td>
       <td>17205</td>
    </tr>
  </tbody>
</table>

### SMOTE Oversampler
### ClusterCentroids Undersampler
### SMOTEENN

### Analysis

## Ensemble Learning

### Balanced Random Forest Classifier

### AdaBoosting

### Analysis
