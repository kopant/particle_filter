# particle filters for map matching

Cheryl Roberts (kopant@gmail.com)  
<br>
This project includes a class for fitting particle filters to GPS trace data, adapted from 
Newson and Krumm's 2009 paper "Hidden Markov map matching through noise and sparseness." 
That paper used HMMs to smooth GPS traces, whereas here I have used particle filters.

One difference in my approach is that as I do not have easy access to the driving distance between two arbitary points, I use haversine distance in the transition calculation. 

Code has been tested with python 3; an environment.yml file lists the dependencies.

## Datasets
1. Cabspotting GPS trace data, retrieved from http://crawdad.org/epfl/mobility/20090224/cab/
2. San Francisco shapefile, retrieved from OpenStreetMap via https://extract.bbbike.org

## References
1. Newson, P. and Krumm, J. (2009). Hidden Markov Map Matching Through Noise and Sparseness. Proceedings of the 17th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems, Seattle, WA, pp. 336-343. 
2. Russell, S. and Norvig, P. (2009). Artificial Intelligence: A Modern Approach (3rd Edition). Pearson: London, UK. 
