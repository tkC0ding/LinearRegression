# Linear Regression From Scratch

- In this project I have implemented a basic supervised learning algorithm, Linear Regression
- I have used pandas to read the dataframe and matplotlib to plot the graphs for prediction and depiction of change of loss

### Linear Regression Intuition

The basic Intuition for linear regression is a straight line which is at the most minimal distance from all the datapoints.

> h(x) = &theta;<sub>0</sub> + &theta;<sub>1</sub>x

where _**&theta;<sub>1</sub>**_ is the slope of the line and _**&theta;<sub>0</sub>**_ is the y intercept of the line

### Error Function

The error function also called the cost function used is **Squared Error Function**

The loss function is basically the summation of the square of the difference between the hypothesis and the original value

>  J(&theta;<sub>0</sub>, &theta;<sub>1</sub>) = 1 / 2m  <sub>i=1</sub>&sum;<sup>m</sup> ( h( x <sup>i</sup> ) - y <sup>i</sup> ) <sup>2</sup>

### Gradient Descent

The error function is a convex function means it forms a bow type function in 3D. If we view it in 2D it is a parabola with an upward open. To reduce this error and reach the minimum point gradient descent optimizer is used.

> &theta;<sub>j</sub> := &theta;<sub>j</sub> - &alpha; (∂ / ∂ x ( J ( &theta;<sub>0</sub>, &theta;<sub>1</sub> ) ))

where &alpha; is the learnning rate

>Note:I have not explained everything in detail, please refer to Andrew Ng's course video for the proper explanation

> The code runs on WSL(Windows Subsystem for Linux) &therefore; the directory structure is based on WSL (/mnt/c/...)
>I have used the salary dataset from kaggle
>
>Here are the [graphs](https://github.com/tkC0ding/LinearRegression/blob/main/Graphs/)


- To run the code on your system, it is required to install WSL on your system as the directory structure used in the project is WSL
- Create a folder called MachineLearning in C: and clone the repo inside the folder
- If you want to clone in a different folder then u need to change the directory for accessing the data in LinearRegression.ipynb file
- Change the directory on the line df = pd.read_csv(...) 