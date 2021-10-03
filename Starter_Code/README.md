# Challenge_week_14

This is a Jupyter Notebook for machine learning trading.

---

## Technologies

This project leverages python 3.7 with the following packages:

* [pandas](https://github.com/google/pandas) - Flexible and powerful data analysis / manipulation library for Python
* [numpy](https://github.com/google/numpy) - is a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.
* [hvplot](https://github.com/google/hvplot) - provides a high-level plotting API built on HoloViews that provides a general and consistent API for plotting data


---

## Installation Guide

Before running the application first install the following dependencies.

```python
  pip install pandas
  pip install numpy
  pip install hvplot
 
```

---

## Usage

To use the housing application simply clone the repository and run the **machine_learning_trading_bot.ipynb** with:

```python
machine_learning_trading_bot.ipynb.ipynb
```


## Conclusions


It seems that running our predictor would generate us less returns thant the original returns (data from 2015-01-21 to 2015-01-22, SMA inputs 4 & 100) , please see: (http:images/baseline_prediction.png)

It seems that running our predictor during a smaller period of time makes our predictions have higher returns during most of the run time (data from 2018-01-21 to 2015-01-22, SMA inputs 4 & 100) , please see: (http:images/tuned_prediction_date_modified.png)

It seems that running our predictor during a smaller period of time makes our predictions have higher returns during most of the run time, although increasing the SMA values doesn't seem to have a big impact, and if anything, it would be a negative impact in this case (data from 2018-01-21 to 2015-01-22, SMA inputs 50 & 200) , please see: (http:images/tuned_prediction_date_and_sma_modified.png)

It seems that running our predictor with a linear regression does not have a significant impact on the prediction, further test with other prediction models is needed, please see: (http:images/lr_tuned_prediction.png)

## summary evaluation report 

As a summary of our tests, is seems that using 3 years of data for our prediction and lower SMA values gives us a very reasonable prediction, as the model results are higher than the actual returns without the model, although it does fall below at the end period. As such, it would require some further testing to tune the model to make it perform above the actual returns in a consistent way.

## Contributors

Brought to you by Rodrigo Monge.

---

## License

N/A