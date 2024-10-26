  The program impliments the Parzen Rosenblatt Kernel smoother on an Multimodal distribution. 
  Aswell, performs bias variance ananlysis in the following steps: 
  
    1.) generate 150 samples from the population distribution 
    
    2.) evaluates the KDE on each sample at a given h bandwidth 
    
    3.) finds the bias and variance of the trials for each bandwidth 
    
    4.) plots the totall bias and variance of the KDE as a function of step size 
    
    5.) evaluates the MSE and prints MSE (sum of totall bias and variance) to suppliment visual plot 


  Example usages:
  the KDE evaluated on 1 sample at a vareity of h values plotted with the true distribution
![alt text](https://github.com/Jacob-J-Richards/R_Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/better.png)

  totall bias and variance of the KDE as a function of step size performed on 150 samples from distribution 
![alt text](https://github.com/Jacob-J-Richards/R_Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/better2.png)
![alt text](https://github.com/Jacob-J-Richards/R_Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/better3.png)


  Plot of the mean of each output at each alpha of the 150 samples and evaluations  
![alt text](https://github.com/Jacob-J-Richards/R_Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/better5.png)

