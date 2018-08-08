# Chapter 2: Supervised Machine Learning
>Machine Learning is a field of Mathematics and Computer Science, that gives Machines or Computers the ability to learn. - Wikipedia

Now, that was an obvious definition, but what does it mean??? In order to understand Machine Learning, let us consider a real-life example. Let us imagine that we have the temperature data for 7 days and we wish to predict what would the temperature would be like on the eighth day. Let us first consider the following imaginary data:
```
Days  Temperatures
1          32.4
2          34.6
3          32.7
4          32.6
5          32.8
6          32.9
7          33.1
```
![Plot of Temperature against Days](https://github.com/koderunners/Machine-Learning-MOOC/blob/master/1_Introduction_to_Machine_Learning/Assets/figure_1.png)

From the above visualization, we can see that the temperature increases almost linearly with the passing days. Thus we can approximate the temperature to be a linear function of the number of days, i.e, if we consider the temperature to be ```y``` and number of days to be ```x```, then the linear function can be represented as ```y = m * x + c```, which is basically the equation of a straight line where ```m``` is the slope of the line and ```c``` is the y-intercept of the line. We need to find the straight line which fits the given data best, i.e, the value of ```m``` and ```y``` for which the line is the best fit for the best data. Once we have the optimal value of ```m``` and ```c```, we can simply plug the value of ```x```, which is the eighth day in this case and get the predicted temperature on that day. This type of prediction algorithm is called **Linear Regression**.

![Plot of Temperature against Days with Linear Regression](https://github.com/koderunners/Machine-Learning-MOOC/blob/master/1_Introduction_to_Machine_Learning/Assets/figure_2.png)

The above plot is an example of Linear Regression, the red line representing the plot of the linear function with optimized parameters(```m``` and ```c```).
**Regression** is a statistical method of estimating the relationship between variables and involves prediction of a **real value**. The above problem of predicting temperatures is called **Univariate Lienar Regression**, since the **dependent variable** is dependent on only one **independent variable**, i.e, the number of days. In reality, the temperature on a particular day is not just dependent on the number of days, but also lots of other factors(variables) such as humidity, precipitation, cloud cover, etc. If we consider more than one variable that affects the value of the dependent variable while applying linear regression, it is called **Multivariate Linear Regression**, i.e, Linear Regression done with multiple variables. This is a more commonly used regression method than Simple Linear Regression because in real life, the outcome of something rarely depends on just one factor.

![Plot of Temperature against Days with Linear Regression](https://github.com/koderunners/Machine-Learning-MOOC/blob/master/1_Introduction_to_Machine_Learning/Assets/figure_3.png)

**Examples of Real World Regression Problems:**
1. [House Price Prediction](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
2. [New York City Taxi Fare Prediction](https://www.kaggle.com/c/new-york-city-taxi-fare-prediction)

Linear regression can not only be done on linear features, but also be used on polynomial features which lets the model learn more complex functions such as the one shown above.
Regression problems are a subset a type of Machine Learning problems known as **Supervised Learning** problems. In Supervised Learning, we train an algorithm which learns the function that best approximates the relation between the input data (independent variable) and the given output data (dependent variable).
Besides Regression, **Classification** is another type of Supervised Learning problem in which the algorithm predicts **discrete values** or **classes** instead of real values. Classification problems are widely used in real world in many applications, for example, classifying spam and non-spam emails, classifying and identification of images, object detection, face recognition and many other applications.
**Examples of Real World Classification Problems:**
1. [Digit Recognizer](https://www.kaggle.com/c/digit-recognizer)
2. [Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)
