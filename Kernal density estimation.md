## Kernal density estimation

Kernal density estimation is similar to the quadrat method where the number of points within a given window is counted to calculate density. However, the different is that this window is allow to move and points that occur further away get a lower weight in the kernal function. For example, a density is calculated for each cell but based on a 4x4 grid around each cell. If a point is located in the outer box it is given less weight in the estimation. 

# KDE gives a more smoothed density than the basic quadrat method and is often used to produce heat maps. NB. Heat maps are different from hot spot maps as they are based on occurance of events rather than attribute values of polygons. 

# Is this not the same as interpolation?

Interpolation is used where it is theoretical possible to take a measurement of an attribute value, eg. soil sample. This is not necessarily the case for crime events in the sense that there may not have been any occurences of crime. 
