# AE-with-Continuous-Bernoulli

An AE on my custom cats and dogs dataset, this time using the continuous bernoulli log loss from 1907.06845. 

Previously (in a different repo), we have used the mse loss on the same AE architecture. The dataset is not adequate to hope for a good performance on validation/test sets, however even on the training dataset, the results are much worse when using the continuous Bernoulli likelihood as the loss function than when we simple use mse. The images are blurry and the colours are washed out. 
