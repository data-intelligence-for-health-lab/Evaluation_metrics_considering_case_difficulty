# Prediction Performance Metrics Considering Case Difficulty Project
This project introduces novel prediction performance metrics that consider case difficulty. These novel performance metrics reward models for correct predictions on difficult cases and penalize them for incorrect predictions on easy cases. The prediction difficulty of individual cases is measured using three different case difficulty metrics (CDmc, CDdm, and CDpu) as described in our [previous research](https://github.com/data-intelligence-for-health-lab/Measuring_Case_Difficulty.git). This project evaluates seven machine learning models, both with and without considering the difficulty of individual cases.

## Datasets

The case difficulty values for the datasets listed below can be found in our previous research:
- **Simulated datasets**: Isotropic Gaussian blobs and interleaving crescent moon datasets
- **Real-world datasets**: Original UCI Wisconsin Breast Cancer data, Telco Customer Churn data, and customer segmentation.

## Machine Learning Models
The following machine learning models are evaluated:
- k-nearest neighbors (knn)
- logistic regression (lr)
- support vector machine (svm)
- naive bayes (nb)
- random forest (rf)
- shallow neural network (snn)
- deep neural network (dnn)

## Evaluation Metrics
The code provides the following results when case difficulty is considered or not:
### Binary Classification Metrics
- Accuracy
- Sensitivity
- Specificity
- Positive Predictive Value (ppv)
- Negative Predictive Value (npv)
- Receiver Operating Characteristic Area Under the Curve (roc_auc)

### Multiclass Evaluation Metrics
- Micro-average accuracy
- Micro-average sensitivity
- Micro-average specificity
- Micro-average ppv
- Micro-average npv
- Micro-average auc
- Macro-average accuracy
- Macro-average sensitivity
- Macro-average specificity
- Macro-average ppv
- Macro-average npv
- Macro-average auc

**Note:** CDmc, CDdm, and CDpu were originally named Approach 1, Approach 2, and Approach 3, respectively. Some code results may still refer to the previous names.