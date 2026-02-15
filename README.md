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

<img width="506" height="532" alt="template_face_detection" src="https://github.com/user-attachments/assets/3b26c988-35a9-47c8-b5a2-e71d9200bbce" />


###  Group Face Detection
<img width="1596" height="1094" alt="Group_detection (1)" src="https://github.com/user-attachments/assets/44be42f7-9acd-41fd-98fb-0baee6a4eb92" />



###  Initial Cluster Plot
<img width="1294" height="697" alt="Cluster_plot" src="https://github.com/user-attachments/assets/a629bfb1-ea4a-4774-ad5c-58ace3d544aa" />



###  Final Cluster Plot with Shashi Taroor
<img width="1286" height="708" alt="Cluster_plot_Shah_taroor" src="https://github.com/user-attachments/assets/6ba9b021-87fb-44ca-b129-e8b0aa4713ef" />



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




