# air_pollution_mortality_ML

Project: Comparison of PCA and autoencoders using time series data of premature deaths due to air pollution from countries worldwide

Team:
Sophie Logan
Rodrigo Salazar

Problem
We want to forecast premature deaths caused by air pollution in countries worldwide using time series data and modeling with PCA and auto-encoders.
In 1992, Lee and Carter, successfully forecasted US Mortality using SVD. Their paper became a reference for using SVD with model demographic data. Given the nature of our data, premature deaths, we have decided to use their work as reference to build our model. In other papers, other factors have been incorporated when modeling demographic data using SVD, like effects of HIV, conflict, and natural disasters. In our case we want to incorporate the presence of high levels of particulate matter, and we are considering incorporating other features like GDP or health expenditure. 
We are going to start by building a PCA model. Our rows will correspond to every year in our data. Then, one of our parameters is going to be a shift between our features and the premature deaths. We want to see which shifts give us a higher accuracy, as deaths due to air pollution are not immediate. 
After building a robust PCA model, we will explore modeling with auto-encoders, as they are capable of catching non-linear relationships in our data. We have seen that this technique has mostly been applied to image or sound recognition. We want to explore its performance with time series. The second paper that we took as reference used PCA and different types of autoencoders for cancer subtype detection. Including: vanilla, sparse, denoising, and variational. For this reason we wanted to use it as a reference. 
Finally, once we have the results, we would like to see how well our models perform, and especially, if autoencoders did better than PCA.
Data
We have data from >100 countries with pollution levels and premature deaths since 1990. The data is from OECD and has few missing values. Most of the other variables that we are planning to use are from the same source, such as health expenditure and GDP. 
Initial Literature Review
Paper 1: 
Lee, Ronald D., and Lawrence R. Carter. “Modeling and Forecasting U. S. Mortality.” Journal of the American Statistical Association 87, no. 419 (1992): 659–71. https://doi.org/10.2307/2290201 

Paper 2:
Franco, Edian F., Pratip Rana, Aline Cruz, Víctor V. Calderón, Vasco Azevedo, Rommel T. J. Ramos, and Preetam Ghosh. 2021. "Performance Comparison of Deep Learning Autoencoders for Cancer Subtype Detection Using Multi-Omics Data" Cancers 13, no. 9: 2013. https://doi.org/10.3390/cancers13092013 
