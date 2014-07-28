Coursera Practical ML Project
=========

The goal of the project is to predict the manner people exercised - they were asked to perform barbell lifts correctly and incorrectly in 5 different ways. The features come from their activities data - accelerometers on the belt, forearm, arm, and dumbell.

>To check the results, download `project_final.html`.
>The data for this project come from this source: http://groupware.les.inf.puc-rio.br/har.

 
### How was it done

The program was coded in `R` using the `caret` package.

* Data cleaning: removed columns with `near zero variance` and with lots of NA.
* Feature selection: performed with `PCA`, using threshold of 0.9 (hold ~90% of the variance). 18 variables were selected this way.
* Model: used `Random Forest` with 25 trees.
* Methodology: performed `10 fold cross-validation` 10 times to tune the parameters and get out-of-sample error estimation.
* Both in-sample and cross-validation accuracy  of the model were ~0.99. `The test set accurary was 0.962`.
* The model got the 20 submission test cases correctly.

