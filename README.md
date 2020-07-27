# Supervised Learning

## Overview

## Logistic Regression Results Using Different Sampling Techniques



### Random OverSampler

#### Target Resampled
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
       <td>0.60</td>
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
       <td>0.71</td>
       <td>0.92</td>
       <td>0.78</td>
       <td>0.62</td>
       <td>17205</td>
    </tr>
  </tbody>
</table>



### SMOTE Oversampler

#### Target Resampled
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
        <td>0.7966770207605626</td>
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
      <td>2042</td>
      <td>15076</td>
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
      <td>0.03 </td>
      <td>0.71</td>
      <td>0.88</td>
      <td>0.06</td>
      <td>0.79</td>
      <td> 0.62</td>
      <td>87</td>
    </tr>
    <tr>
      <td>low_risk </td>
      <td></td>
      <td>1.00</td>
      <td>0.88</td>
      <td>0.71</td>
      <td>0.79<0.94/td>
      <td>0.64</td>
      <td>17118</td>
    </tr>
    <tr>
      <td>avg / total</td>
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



### ClusterCentroids Undersampler

#### Target Resampled
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
      <td>260</td>
      <td>260</td>
    </tr>
  </tbody>
</table>

##### Balanced Accuracy Score
<table>
  <tbody>
    <tr>
        <td>0.7752245065690078</td>
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
       <td>68</td>
       <td>19</td>
    </tr>
    <tr>
      <td>Actual False</td>
      <td>3957</td>
      <td>13161</td>
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
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
    </tr>
    <tr>
       <td>low_risk </td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
    </tr>
    <tr>
       <td>avg / total</td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
    </tr>
  </tbody>
</table>



### SMOTEENN

#### Target Resampled
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
      <td></td>
      <td></td>
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
       <td></td>
       <td></td>
    </tr>
    <tr>
      <td>Actual False</td>
      <td></td>
      <td></td>
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
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
    </tr>
    <tr>
       <td>low_risk</td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
       <td></td>
    </tr>
    <tr>
       <td>avg / total</td>
       <td></td>
       <td></td>
       <td></td>
       <td>/td>
       <td></td>
       <td></td>
       <td></td>
    </tr>
  </tbody>
</table>

### Analysis

## Ensemble Learning

### Balanced Random Forest Classifier

### AdaBoosting

### Analysis
