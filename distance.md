# Distance based methods

## Nearest Neighbour

Method to establish the extent of clustering using distance of points to their nearest neighbour. The average distance of randomly selected points to their nearest neighbour is divided by the expected distance which by some fiddly integration can be shown is.

![equation](https://latex.codecogs.com/gif.latex?\bar{r_{E}}&space;=&space;\frac{1}{2\sqrt{\lambda}})

The R index is just 

![equation](https://latex.codecogs.com/gif.latex?R&space;=&space;\frac{\bar{r_{A}}}{\bar{r_{E}}})

You can also test that mean observed distance follows CSR by subtracting observed distance from expected distance and divide by standard deviation to get z score.


NN index = 0 Clustered

NN index = 1 Random

NN index > 1 Uniform

## Ripley's K function

Ripley's k function builds on the nearest neighbourhoods method but the key difference is that it considers multiple neighbours. In fact it counts the number of neighbors within multiple distance bands from each event/point. The average number of points for each distance band is calculated with these values standardized by dividing by the density of points within the whole area. This is compared with the expected value of k(d) under complete spatial randomness. 

Expected value of K(d) is

![equation](https://latex.codecogs.com/gif.latex?E\left&space;[&space;K\left&space;(&space;d&space;\right&space;)&space;\right&space;]&space;=&space;\frac{\lambda&space;\pi&space;d^{2}}{\pi&space;}&space;=&space;\lambda&space;d^{2})

In fact, as the expected and observed functions become large, it is often better to convert the expected value of K(d) to 0 using the following formula. 

![equation](https://latex.codecogs.com/gif.latex?L(d)&space;=&space;\sqrt{\frac{K(d)}{\pi&space;}}&space;-&space;d)
