# Geotagged-Photo-Clustering-using-DBSCAN

This project focuses on identifying and visualizing popular geographic locations by clustering geotagged photographs using the DBSCAN (Density-Based Spatial Clustering of Applications with Noise) algorithm. By extracting GPS metadata embedded in image files through the EXIF format, the system converts raw latitude and longitude data into a structured dataset using Python libraries such as exifread, pandas, and numpy. The extracted coordinates are normalized via StandardScaler to prepare the spatial data for clustering.
It has practical applications in tourism analytics, event detection, and geographic information systems (GIS), providing a scalable and automated method for identifying popular locations through the lens of photographic behavior.

# Installation and Setup
To ensure the project runs smoothly across different systems, the following setup is required:
1.	Install Python 3.x (if not already installed).
2.	Set up a virtual environment (recommended):
<img width="895" height="105" alt="image" src="https://github.com/user-attachments/assets/c79b3c0b-98b0-43dc-aa13-bf355e87b4b9" />
 
3.	Install dependencies using pip:
<img width="895" height="87" alt="image" src="https://github.com/user-attachments/assets/b1409109-5163-4916-bb21-928f5d81ebeb" />

4.	Run the script/notebook on Jupyter Notebook or Google Colab:
- Upload sample images (for Colab) or set local folder paths (for Jupyter).
- Execute cells sequentially to extract GPS data, run DBSCAN, and visualize the clusters on a map.

# Tool Setup
A robust Python-based environment was configured for developing and testing the clustering system.
- Programming Language:
Python (version 3.8+) was used due to its rich ecosystem of data science, machine learning, and geospatial libraries.

- Libraries and Tools Used:
1. pandas and numpy for data manipulation
2. exifread or Pillow for EXIF metadata extraction
3. scikit-learn for DBSCAN clustering and preprocessing
4. matplotlib, seaborn, and folium for data visualization
5. os, glob, and pathlib for file system access
   
- Development Platform:
Jupyter Notebook was used for initial experimentation and analysis. The final scripts were packaged into Python modules or Streamlit apps.

- Version Control:
Git and GitHub were used to manage code versions and ensure reproducibility.

# 📊 What You Get
	- A CSV file (clustered_locations.csv) showing each image and its cluster.
	- An interactive map (geotagged_clusters_map.html) showing clusters of photos.
	- Red dots = noise/outliers
	- Colored dots = clustered photo locations
