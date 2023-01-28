# Landcover-use-analysis
Land-cover classification is a type of semantic
segmentation in which an RGB image of a given
area is segmented based on different
landcovers.We have use Sentinel-2 data from AWS and processed the geotiff 
format accesible for analysis and deep learning models.
We have used different kind of Dimensionality reduction techniques like PCA and TSNE's to 
reduce the dimensionality and finally model the data using CNN.


CONCLUSION

For the given location, in the past 5-6 years, there haven't been much change like urban expansion, deforestation/afforestation, etc. In fact,
its hard to find places, where just in 5-6 years there are considerable changes in land-use. Also, the SENTINEL program started in 2016, so
we are restricted to years after that. If we go to LANDSAT satellite images, there resolution in 30m and can never be used for semantic
segmentation or classification.
But overall, the performance of our model is good enough, as the mean value of percentage land-use is almost correct as it appears from
the above images.
The places where improvement can be done is training our model on more and more images (we tried labelling our own dataset but due to
time constrained didn't continue with that). Also, there can be some improvement in how we are accessing the data. We can use a model for
cloud detection in images and filter images based on cloud cover too. These work will surely improve our results but the major constrain is
the quality of image. SENTINEL-2 gives 10m resolution, this any change in land-use which is below the size of 100m^2 wont be even visible.
Thus, with better satellite images, our model and pipeline can be very useful.
