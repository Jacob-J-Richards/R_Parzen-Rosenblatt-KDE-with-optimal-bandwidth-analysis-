  The program impliments the Parzen Rosenblatt Kernel smoother on an Multimodal distribution. 
  Aswell, performs bias variance ananlysis in the following steps:
  
    1.) generate 150 samples from the population distribution 
    
    2.) evaluates the KDE on each sample at a given h bandwidth 
    
    3.) finds the bias and variance on the aggreagate of the trials for each bandwidth 
    
    4.) plots the totall bias and variance of the KDE as a function of step size 
    
    5.) evaluates the MSE and confirmes the visual results of the visual plot that 
    h = 0.6 is the opitmal choice. 

  The conlusion drawn from this implimentation is that a step size of h = 0.6 is optimal 
  for the given distribution being aproximated

  the KDE evaluated a variaity of h values plotted against the true distribution 
![alt text](https://github.com/Jacob-J-Richards/R_Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/better.png)

  totall bias and variance of the KDE as a function of step size 
![alt text](https://github.com/Jacob-J-Richards/R_Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/better2.png)
![alt text](https://github.com/Jacob-J-Richards/R_Parzen-Rosenblatt-KDE-with-optimal-bandwidth-analysis-/blob/main/better3.png)

