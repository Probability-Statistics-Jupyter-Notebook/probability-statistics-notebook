# Probability and Statistics Reviewing Notes

Here are Jupyter notebooks of the course Probability and Statistics. 

## Course information

**Korea Advanced Institute of Science and Technology (KAIST).** 

**Course name**: CC511 Probability and Statistics

**Advisor**: Professor. Sung-Ho Kim, Department of Mathematical Science.

**Textbook**: Probability and Statistics for Engineers and Scientists, 4th ed. by A. J. Hayter

## Content

Chapter 1. Probability Theory

Chapter 2. Random Variables

Chapter 3. Discrete Probability Distributions

Chapter 4. Continuous Probability Distributions 

Chapter 5. Normal Distribution

Chapter 6. Descriptive Statistics

Chapter 7. Statistical Estimation and Sampling Distributions

## Environment requirements

```
Python version: 3.8 or later
Python package: scipy, math, jupiter notebook/lab
```

## What we have done

There are two types of notebooks., both of them cover all the content.  

One is mainly used for **learning** this course, with comprehensive definitions and theorems and beautiful codes help you understand the calculating process.  

Another one is mainly used to **review** this course, or works as an answer sheet, with concise summary of knowledge points and practical code to help you get the result. 

### Notebook for Learning

For each chapter, each section, we summarized the important definitions and theorems. These will be shown on the markdown part in each section. 

<img src="./imgs/bertu-definitions.PNG" alt="Definitions" style="zoom:80%;" />

Then, we use Python code to implement the calculation part. With the help of code, you will easily understand the calculating process, which we believe is really important to master and practice the definitions and theorems we learned. 

In each code block, we showed required parameters at the beginning, you can modify them freely with your need, and then get the result you want. 

<img src="./imgs/bertu-code.png" alt="Code" style="zoom:80%;" />

<img src="./imgs/bertu-result.png" alt="Result" style="zoom:80%;" />

Sum up, there are three parts for each section: 

- Definitions and theorems
- Code implement by Python 
- Result output

<img src="./imgs/bertu-sumup.png" alt="Sumup" style="zoom: 67%;" />

### Notebook for Reviewing

If you have complete the learning of this course, you may want a more simple notebook to help you review it efficiently. These notebooks are designed for this. 

Similarly, we showed definitions at the beginning of each section, but now these definitions and theorems have been quite concise. Just have a glance to refresh you mind. You can do it. 

<img src="./imgs/chuanbo-definitions.png" alt="Definitiosn" style="zoom:80%;" />

Then, there are code blocks to help you do some calculations. In each cold block, there are three parts: `input`, `calculate` and `output`. 

You can modify values in the `input` freely, and the code will output the result. 

<img src="./imgs/chuanbo-code.png" alt=" " style="zoom:80%;" />

<img src="./imgs/chuanbo-result.png" alt="Result" style="zoom:80%;" />

If you forget the meaning of parameters, it dose not matter, we also note he parameters' definitions there. 

<img src="./imgs/chuanbo-sumup.png" alt="Code" style="zoom: 67%;" />

Since these notebooks are quite simple and clear, you can easily use them to be your answer sheet in exams. That must be amazing helpful.  

## How to use

**Step 1**. Clone the repository to your computer, open the `.ipynb` files with [Jupyter  Notebook](https://jupyter.org/) or [Jupyter Lab](https://jupyter.org/). Or, you can use [Google CoLab](https://colab.research.google.com/) to load them. 

**Step 2**.  Run the first one or two code blocks to set the packages environment. 

![](https://github.com/Probability-Statistics-Jupyter-Notebook/probability-statistics-notebook/blob/master/imgs/chuanbo-head.PNG)

![](https://github.com/Probability-Statistics-Jupyter-Notebook/probability-statistics-notebook/blob/master/imgs/bertu-head.PNG)

If there is something wrong with environment setting, please check you Python and packages' version. 

**Step 3**. Do whatever you want, you can freely modify the parameters in code blocks for your calculation.  

## Contact us 

If you find any bugs, please feel free to create issues, we will deal with them as soon as possible. 

























Notes are written by Jupiter Notebook. Please run the first two code blocks in every notebook for importing package and function definition. 

For each section in the textbook, we summarized the most important definitions and formulas, following by implement with Python code. 

In each code block, 

```python
# Input
mu = 29.4
sigma = 2.1
pdf_variable = [29.0, 30] # [star point, end point]
cdf_variable = 29.4

# Calculate
exp, var = norm.stats(loc=mu, scale=sigma, moments='mv')
pdf = norm.cdf(pdf_variable[1], loc=mu, scale=sigma) - norm.cdf(pdf_variable[0], loc=mu, scale=sigma)
cdf = norm.cdf(cdf_variable, loc=mu, scale=sigma)

# Output
print_status(exp, var, pdf, cdf)
```

You can modify values in the `input` part freely, and the code will output the result. 

- `Exp`: Expectation
- `Var`: Variance
- `PMF/PDF`: Probability distribution function value
- `CDF`: Cumulate distribution function value 