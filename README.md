# Lab 5: Face Detection & Clustering

##  Student Details
**Name:** Phani Srivatsav  
**Roll No.:** U20240118  
**Branch:** CSAI  


## Objective
The goal of this lab is to detect faces in images and group similar faces using clustering techniques.  
We use OpenCV for face detection and K-Means clustering to group faces based on color features.


##  Tools & Libraries Used
- Python
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn (KMeans)

---

##  Methodology

###  Face Detection
- Used Haar Cascade Classifier.
- Detected faces in a group image.
- Drew bounding boxes around each detected face.

### Feature Extraction
- Converted each face to HSV color space.
- Extracted:
  - Mean Hue
  - Mean Saturation
- These values represent each face numerically.

### Face Clustering
- Applied K-Means clustering with **K = 2**.
- Grouped faces based on similarity in color features.
- Calculated cluster centroids.

### Template Face Classification
- Detected face in the template image.
- Extracted its Hue & Saturation.
- Assigned it to the closest cluster.


## Results & Visualizations

###  Template Face Detection
![Template Face Detection](template_detection.png)


###  Group Face Detection
![Group Face Detection](group_detection.png)


###  Initial Cluster Plot with Template
![Initial Cluster Plot](cluster_plot.png)


###  Final Cluster Plot with Template
![Final Cluster Plot](Cluster_plot_Shahi_taroor.png)


## Observations
- Haar Cascade successfully detected most faces.
- Hue and Saturation provided a simple way to compare faces.
- K-Means grouped faces into two clear clusters.
- The template image was assigned to the nearest cluster.


##  Conclusion
This lab demonstrates how basic computer vision and clustering can work together.

Key takeaways:
- OpenCV can efficiently detect faces.
- HSV color features help compare faces.
- K-Means clustering groups similar faces.
- New images can be classified using learned clusters.




