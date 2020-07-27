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


<table>
  <thead>
    <tr>
      <th>SMOTE</th>
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

<table>
  <thead>
    <tr>
      <th>ClusterCentroids</th>
      <th>Predicted True</th>
      <th>Predicted False</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>Actual True</td>
       <td>68</td>
       <td>68</td>
    </tr>
    <tr>
      <td>Actual False</td>
      <td>3957</td>
      <td>13161</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>SMOTEENN</th>
      <th>Predicted True</th>
      <th>Predicted False</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>Actual True</td>
       <td>72</td>
       <td>15</td>
    </tr>
    <tr>
      <td>Actual False</td>
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
      <th>Pre</th>
      <th>Rec</th>
      <th>Spe</th>
      <th>f1</th>
      <th>Geo</th>
      <th>IBA</th>
      <th>Sup</th>
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
      <th>Pre</th>
      <th>Rec</th>
      <th>Spe</th>
      <th>f1</th>
      <th>Geo</th>
      <th>IBA</th>
      <th>Sup</th>
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
      <th>Pre</th>
      <th>Rec</th>
      <th>Spe</th>
      <th>f1</th>
      <th>Geo</th>
      <th>IBA</th>
      <th>Sup</th>
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
      <th>Pre</th>
      <th>Rec</th>
      <th>Spe</th>
      <th>f1</th>
      <th>Geo</th>
      <th>IBA</th>
      <th>Sup</th>
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
      <th>Predicted True</th>
      <th>Predicted False</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>Actual True</td>
       <td>64</td>
       <td>23</td>
    </tr>
    <tr>
      <td>Actual False</td>
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
      <th>Rec</th>
      <th>Spe</th>
      <th>f1</th>
      <th>Geo</th>
      <th>IBA</th>
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
      <th>Predicted True</th>
      <th>Predicted False</th>
    </tr>
  </thead
  <tbody>
    <tr>
       <td>Actual True</td>
       <td>22</td>
       <td>65</td>
    </tr>
    <tr>
      <td>Actual False</td>
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
      <th>Pre</th>
      <th>Rec</th>
      <th>Spe</th>
      <th>f1</th>
      <th>Geo</th>
      <th>IBA</th>
      <th>Sup</th>
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
