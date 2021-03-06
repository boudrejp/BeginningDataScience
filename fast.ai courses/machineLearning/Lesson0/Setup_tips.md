# Tips before starting

### General notes
* We are trying to get a normally 12 week course done in about 3 weeks. Because of that, we're not going to go into as much detail with work outside of lectures, but I still think we can learn a lot here.
   * The idea here is not to make you an expert in one course, but to get you hands on experience such that you would know how to learn more if you so choose. Or, for those of us in Berkeley, becoming used to performing machine learning analyses using python ahead of W207.
* Overall, the goal for each lesson here is going to be:
   * Watch the lectures and don't worry too much if you don't understand everything on the first go
   * Pick your own dataset to replicate the analysis done in class (adapt the code where needed for this, but maintain the same overall structure)
      * I will provide a few examples of sample data sets that should perform similarly to those presented in class if you don't have one that you already have in mind
   * We will have virtual sessions of all of us together to share the progress we've made on our independently chosen data set to learn from those approaches and reinforce what's been done, ask questions, etc
* We have RocketChat as a collaboration forum for questions, banter, updates, etc

### Python
* This course will be using Python 3. In Python, there is "base" functionality that is written in the Python language, and there are pre-written Python libraries that can be imported and used. This class will be making heavy use of pre-written libraries to make using the various machine learning topics easy to implement.
* Common libraries for data science include numpy (optimized array computations), pandas (built on top of numpy, allows you to have data tables which function similar to excel/ R data frames), and sklearn (implemented machine learning algorithms and associated functionality).
* In python, it's common to see long lines of code with many dots. Because Python is an object oriented language, functions can be written as methods for types of objects. If this is confusing, don't worry about it too much - this basically just means that any code following a dot means that the proceeding code is applied to the code before the dot. For example...
  * `df["sales"].groupby(df.productcode).mean()`
* A crash course on Python for data science can be found here: https://www.listendata.com/2017/05/python-data-science.html
* A crash course for more general python can be found here: http://pythonentresdias.blogspot.com/p/who-serves-this-blog-learn-python-in.html
* __Overall, don't worry so much about being able to write your own code from scratch. We'll use the class examples with minor tweaks to understand the material better__

### Jupyter
* Jupyter notebooks are a convenient way to run Python code. The code is written into cells which can be executed independently of one another.
* They can also be configured to run R and Julia code, but we will stick with Python for this class.

### Crestle
* The course has a pre-configured cloud service for running Jupyter notebooks with a GPU for a compute engine called crestle.
* I recommend that everyone makes an account here and uses this. It will be pre-configured with the data needed for the course, and should also have the class notebooks already on there. This will also save us any headaches of replicating environments.
* Note that crestle will charge you $0.30 USD per hour of use of the machines. I doubt that you will use over $20 over the duration of this course.
* Crestle: https://www.crestle.ai/

### Github
* There is a github repo for all the course materials. Might be useful to peruse them outside of Crestle to not get charged.
* repo: https://github.com/boudrejp/fastai/tree/master/courses/ml1

