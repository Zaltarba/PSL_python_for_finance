<img src="https://dauphine.psl.eu/fileadmin/_processed_/9/2/csm_damier_logo_Dauphine_f7b37a1ff2.jpg" width="200" style="vertical-align:middle" /> <h1>Master 222: Introduction to Python </h1>

Welcome to you all !

This [GitHub Home page](https://github.com/Zaltarba/PSL_python_for_finance) contains all the materials for the course **Introduction to Python 2025** at Université Paris Dauphine.

## Getting Started
* The scripts are written as Jupyter notebooks and run directly in Google Colab.
* For those who'd like to execute the scripts locally, consider using Jupyter Notebook. Check out this [tutorial](https://test-jupyter.readthedocs.io/en/latest/install.html) on how to install Jupyter through Anaconda for detailed guidance.

## Learning Outcomes 

The objectives of this module are:
* Grasp foundational Python programming concepts, including variables, data types, and the print() function.
* Master the use of conditional statements (if, elif, else) to control program flow based on specific conditions. 
* Understand the concept and importance of libraries and modules in Python, introducing primary tools like Numpy and Pandas.
* Acquire proficiency in using Numpy for numerical operations and Pandas for structured data exploration, manipulation, and analysis.
* Develop the skills to create and customize data visualizations using Matplotlib, showcasing insights from datasets.
* Introduce yfinance to fetch and analyze stock market data, integrating its functionality with Pandas and Matplotlib for comprehensive financial analysis.

## Assessment 

*Final Exam* : 50%   
*Group Project* : 50% 

### Group Projects Instructions

Projects will be implemented in Python and hosted on GitHub.
Each group (3–4 students) will design and develop a financial trading strategy, split into two parts.

1. Strategy Research & Backtesting
    - Theoretical explanation 
    - Backtest implementation 
    - Both inside in a Jupyter Notebook.
2. Production-Ready Code 
    - A main.py script to generate daily trading signals or outputs.
    - The code must when execute be able to fetch data and save a portfolio weigths files

### Evaluation 

Each group will deliver a 20-minute presentation at the end of the project.

The presentation should clearly explain:  
    - The motivations behind the strategy  
    - The design choices and modeling process  
    - Backtesting results and performance metrics  
    - Lessons learned, limitations, and potential improvements.  

Presentations will be followed by Q&A from instructors.

Students may choose their own strategy or select from the following proposals:

### Suggested Strategies  

1. Trend Following Strategy with Moving Averages (Long-Only) : 
    - Implement a strategy using two moving averages: a short-term (e.g., 10-day) and a long-term (e.g., 90-day).  
    - A long position is opened when the short MA crosses above the long MA, and closed when it crosses below.

2. Momentum Strategy (Long/Short) :
    - Based on the idea that recent winners will continue to perform well. Assets are ranked by recent performance (e.g., over 30 days). 
    - Long positions are taken in top performers, and short positions in the worst performers.

3. Volatility-Based Strategy using GARCH Model (Long/Short)
    - Utilize the GARCH model to forecast volatility and design a trading strategy that reacts to periods of predicted high or low volatility. The model captures asymmetric volatility shocks (leverage effect).

4. Neural Network-Based Prediction Strategy (Long-Only)
    - Build a neural network model to predict the probability of a positive return for each asset. 
    - If the predicted probability exceeds 50%, initiate a long position. No short positions are used.

5. Mean Reversion via Pairs Trading and Hurst Exponent (Long/Short)
    - Identify historically correlated asset pairs and calculate the Hurst exponent of their spread. 
    - A Hurst exponent bellow 0.5 suggests mean-reverting behavior. Trade the pair based on the deviation of the spread from its mean.

## Recommended Reading

*Python for Algorithmic Trading : From Idea to Cloud Deployment* by Yves Hilpisch

[GARCH model tutorial](https://zaltarba.github.io/blog/BitcoinVolatility-2/)

[Fetching Binance Data Tutorial](https://zaltarba.github.io/blog/DataBaseCreation/)
