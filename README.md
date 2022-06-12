SANDISON, 2021: FAFINDER - First Ascent Finder, Version 1 

OVERVIEW:
This script generates locations of potential rock crags for either boulder or sport climbing that
are unexplored and unestablished. Users who find locations of interest can explore these potential rock crags
in person and at their own risk, where hopefully first ascents of undiscovered rock walls can take place.
Using publicly available datasets, it outlines locations where both high slope and rock formations exist 
within a set buffer. Citations for all datasets employed are available in the Earth Engine catalogue.

Identification of rock cover in a given area is completed by a kernelized suport vector machine library 
classifier (libsvm).Pixels with rock cover are buffered to 100m radius to allow overlap with nearby changes in
elevation. A slope layer is also classified the same way (this is a crude work around to convert the layer to 
a vector layer). An intersection command is used to find area's where both buffered rock areas and slope vectors
overlap, producing the 'rock wall' layer.

Visualized website found at: www.fafinder.ca
