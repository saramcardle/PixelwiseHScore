# Pixelwise H-Score
Implementation of Ram, et al., 2021, "Pixelwise H-score: A novel digital image analysis-based metric to quantify membrane biomarker expression from immunohistochemistry images"  (https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0245638). This script calculates the amount of 1+, 2+, 3+ positive pixels in the DAB channel as well as the number of hematoxylin+ pixels to get a total DAB expression score. 

Written by Sara McArdle (La Jolla Institute for Immunology) and Pete Bankhead (University of Edinburgh), 2026. 

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24288085.svg)](https://doi.org/10.5281/zenodo.24288085)



# Usage
1) Set stain deconvolution vectors
2) Set the DAB and Hematoxylin thresholds (lines 4 and 5). Using the QuPath Pixel Thresholder can help visualize the results, but there is no need to save the pixel classifiers.
3) Set the downsample (line 6). Theoretically 1 is best, but higher values make the script run faster.
4) Select your annotations of interest
5) Run this script

# Results
The number of pixels and area above the three DAB thresholds will be written into each annotation measurement. The combined H score will also be written into the measurement list. 

For more information, see these image.sc forum threads: [original](https://forum.image.sc/t/qupath-pixelwise-h-score/79449), [Pete's improvements](https://forum.image.sc/t/implementing-h-score/75041/10?u=smcardle). 
