# Probability_Distributions Package

This package gives the functionality for Gaussian and Binomial probability Distributions.

# Files

`license.txt` - This file contains permissions related to the package usage
`__init__.py` - This file imports necessary classes when you import this package
`Generaldistribution.py` - This python file has the parent class with functionality that can be used in Binomialdistribution and Gaussiandistribution classes
`Gaussiandistribution.py` - This python file defines functionality that can be done with the Gaussian probability distribution
`Binomialdistribution.py` - This python file defines functionality that can be done with the Binomial probability distribution

# Installation

To install this package use the following command:
`pip install Probability_Distributions`

# Usage of the package

## Gaussian Distribution Functions

1. To define a Gaussian distribution with mean m and standard deviation s
`gaussianDistributionName=Gaussian(m,s)`

2. To initialize a gaussian distribution reading in a data efile

`gaussianDistributionName= Gaussian()
 gaussianDistributionName.read_data_file('numbers.txt')`
 
 To Calculate mean and standard deviation of such Distribution
 
 `gaussianDistributionName.calculate_mean()
  gaussianDistributionName.calculate_stdev()`

3. To show the mean of a gaussian distribution
`gaussianDistributionName.mean`

4. To show the standard deviation of a gaussian distribution
`gaussianDistributionName.stdev`

5. To add two gaussian distribution
`gaussian_sum = gaussianDistributionOne + gaussianDistributionTwo`

6. Function to plot the normalized histogram of the data and a plot of the probability density function along the same range
`gaussianDistributionName.plot_histogram_pdf()`

7. Function to calculate the Probability density function for the gaussian distribution at a point x 
`gaussianDistributionName.pdf()`

8. Function to output a histogram of the data
`gaussianDistributionName.plot_histogram()`

## Binomial Distribution Function

1. To define a Binomial distribution with probability p and size s
`binomialDistributionName=Binomial(p,s)`

2. To initialize a gaussian distribution reading in a data efile

`binomialDistributionName= Binomial()
 binomialDistributionName.read_data_file('numbers.txt')`
 
 To Calculate mean and standard deviation of such Distribution
 
`binomialDistributionName.calculate_mean()
 binomialDistributionName.calculate_stdev()`

3. To show the mean of a gaussian distribution
`binomialDistributionName.mean`

4. To show the standard deviation of a gaussian distribution
`binomialDistributionName.stdev`

5. To add two gaussian distribution
`binomial_sum = binomialDistributionOne + binomialDistributionTwo`

6. Function to output a histogram of the instance variable data
`binomialDistributionName.plot_bar()`

7. Function to calculate the Probability density function for the binomial distribution at a point x 
`binomialDistributionName.pdf()`

8. Function to plot the pdf of the binomial distribution
`binomialDistributionName.plot_bar_pdf()`