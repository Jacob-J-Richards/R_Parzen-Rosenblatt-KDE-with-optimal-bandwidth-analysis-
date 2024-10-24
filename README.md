This project implements the Parzen-Rosenblatt Kernel Density Estimator (KDE) and systematically tests for the optimal choice of the bandwidth parameter h. The implementation evaluates the performance of the KDE using simulated data and calculates bias, variance, and Mean Squared Error (MSE) for different bandwidth values.


![alt text](https://github.com/Jacob-J-Richards/Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/prelim.JPG)

Key Features:

Data Generation:
The data is generated from a mixture of four normal distributions with means 0, 3, 6, and 9, respectively, each with a standard deviation of 1. The data is created based on a uniform random variable that assigns the data points to different clusters of these normal distributions.
The generated dataset consists of 800 samples, which are used to evaluate the KDE.

KDE Calculation:
The KDE is computed for a grid of input values ranging from -5 to 10, with a step size of 0.1 (i.e., alpha(1) = -5, alpha(2) = -4.9, etc.).
The KDE evaluates the probability densities at each alpha value using a Parzen window approach, where the bandwidth h is an adjustable parameter.

Simulations:
The KDE is evaluated 150 times, each time with a different set of 800 samples generated from the mixture distribution.
For each simulation, the KDE is computed for all alpha values, resulting in a matrix of evaluations for each trial.

Bias and Variance:
After calculating the KDE for each of the 150 trials, the mean and variance of the KDE estimates are computed at each alpha value across the trials.
The bias at each alpha is computed as the difference between the mean KDE estimate and the true probability density function (PDF), which is known based on the mixture of normal distributions.

Mean Squared Error (MSE):
The MSE is calculated at each alpha value by summing the variance and the square of the bias.
The total bias, total variance, and total MSE are computed by averaging across all alpha values.

Bandwidth Selection:
The KDE is evaluated for different bandwidth values (h), including h = 0.1, h = 1, and h = 7.
By plotting the total bias and variance as functions of h, the optimal bandwidth is determined by minimizing the MSE.
The results confirm that h = 7 yields the lowest MSE for this specific dataset, indicating the optimal choice of bandwidth.

Visualization:
The results are visualized by plotting the KDE estimates for different bandwidths (h = 0.1, h = 1, h = 7) against the true PDF.
Additionally, the bias and variance are plotted as functions of h, demonstrating the trade-off between bias and variance when selecting the bandwidth.

Conclusion:

This implementation explores the trade-offs involved in bandwidth selection for the Parzen-Rosenblatt KDE. It performs simulations to compute the mean, variance, and bias of the KDE across multiple trials and demonstrates that the optimal bandwidth is h = 7, based on minimizing the MSE.

![alt text](https://github.com/Jacob-J-Richards/Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/verified.JPG)

