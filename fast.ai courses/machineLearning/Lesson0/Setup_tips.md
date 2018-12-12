# Tips before starting

### Python
* This course will be using Python 3. In Python, there is "base" functionality that is written in the Python language, and there are pre-written Python libraries that can be imported and used. This class will be making heavy use of pre-written libraries to make using the various machine learning topics easy to implement.
* Common libraries for data science include numpy (optimized array computations), pandas (built on top of numpy, allows you to have data tables which function similar to excel/ R data frames), and sklearn (implemented machine learning algorithms and associated functionality).
* In python, it's common to see long lines of code with many dots. Because Python is an object oriented language, functions can be written as methods for types of objects. If this is confusing, don't worry about it too much - this basically just means that any code following a dot means that the proceeding code is applied to the code before the dot. For example...
  * `df["sales"].groupby(df.productcode).mean()`
