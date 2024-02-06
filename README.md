# AE-with-Continuous-Bernoulli

An AE on my custom cats and dogs dataset. We have two notebooks, one with L2 loss and another with the continuous bernoulli log loss from 1907.06845. 

Observations: The dataset is not adequate to hope for a good performance on validation/test sets, however even on the training dataset, the results are much worse when using the continuous Bernoulli likelihood as the loss function than when we simple use mse. 

Although the reconstructions while using the CB log loss have sharp contrast, it's at the contrast of losing detail and similarity to the originals (eye-test opinion). The sharp contrast values are expected as the norm of the continuous Bernoulli is convex and hence minimising -log p(x) pushes the pixel values to extremes. This is exactly why it produces sharper images when used as a loss in a VAE on MNIST. In the case of colour images, it would needed to be complemented with other loss terms to ensure better similarity in features and colours with the originals.
