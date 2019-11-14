##  Faces Annotation using VIA (VGG Image Annotator).

* Where to get the images?
  * Got the sports images from different news sites. Used the following chrome plugin t - **Fatkun Batch Download Images**- to download the images.  It helps in filtering out the images based on width and height.
* How to annotate the images?
  * [Used VGG Image Annotator (VIA)]('<http://www.robots.ox.ac.uk/~vgg/software/via/>')
  * Create new project
    * Add the images to annotate
    * In the Attribute Section:
      * Define the **region attribute** like class to define. The class value could be a drop down box with list of values.
    * Define the regions and annotate the attributes for all images.
    * Export the project annotations in JSON format.
* [Resized the images using this script.](ResizeImages.ipynb)
* [Clustered the annotated face images using this script](ClusterFaces.ipynb)

The following are the cluster centroids based on log scale of width and height.

```python
array([[ 50.68576131,  67.09112992],
       [ 78.51575295, 105.52204114],
       [138.89936277, 190.13431528],
       [ 31.77059357,  43.23562061]])
```



