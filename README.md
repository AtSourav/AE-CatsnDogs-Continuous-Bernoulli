# AE-with-Continuous-Bernoulli

An AE on my custom cats and dogs dataset. We have two notebooks, one with L2 loss and another with the continuous bernoulli log loss from 1907.06845. 

Observations: The dataset is not adequate to hope for a good performance on validation/test sets, however even on the training dataset, the results are much worse when using the continuous Bernoulli likelihood as the loss function than when we simple use mse. The images are blurry and the colours are washed out. 
