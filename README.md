# Flood Evacuation Network Analysis using QGIS Python

This project presents an **automated GIS-based network analysis workflow** developed in **QGIS using Python**, designed to identify **safe evacuation routes during flood events**. The tool integrates spatial data, network analysis, and cartographic styling to support rapid decision-making in emergency and disaster response contexts.
The workflow focuses on identifying the **fastest or shortest evacuation paths** from flood-affected residential addresses to designated **safety points** (e.g. schools, shelters), while accounting for flood extents, buffer zones, and road network constraints.

## Project Purpose

Flood events require **rapid, repeatable, and reliable evacuation planning**. Manual GIS workflows are often too slow and error-prone during emergencies. This project demonstrates how **GIS automation** can be used to:

⏱️ **Reduce analysis time**  
🔁 **Ensure consistency across scenarios**  
⚡ **Enable rapid re-running of evacuation modelling as conditions change**   

The project is framed as an **applied urban risk and resilience analysis**, suitable for emergency management, urban planning, and spatial decision-support systems.

## What This Project Does

At a high level, the workflow:

1. Identifies flood-affected areas using buffered flood polygons  
2. Selects a user-defined safety point (by name or coordinates)  
3. Clips road networks and address points to the affected study area  
4. Determines which addresses are closest to the selected safety point  
5. Computes the **shortest or fastest evacuation routes** using network analysis  
6. Applies predefined cartographic styles for clear visual interpretation  
7. Outputs both map layers and an exported map image for reporting  



**How to run the codes**
1. Open QGIS and open the code.py file using QGIS Scripts<br/>
![image](https://user-images.githubusercontent.com/80443493/137457987-38bdd4da-ce5e-4514-8abe-0661a9cf565b.png)

2. Run the script <br/>
![image](https://user-images.githubusercontent.com/80443493/137458045-f55cde87-6888-4749-b781-664f4e4d6079.png)

3. Input path to all the files (shapefile and qml) and provide the following details: <br/>
  a. Buffer distance value <br/>
  b. Selected safety point name <br/>
  c. Selected safety point latitude and longitude <br/>
![image](https://user-images.githubusercontent.com/80443493/137458213-41af22e8-dfb5-4f3f-88ab-f726765e1cfa.png)

4. Once the desired layers are loaded, run the export_image.py code using the Python Console <br/>
![image](https://user-images.githubusercontent.com/80443493/137458312-9fb413d9-c716-40bf-af63-7589e1802d66.png)

5. Once the code is executed the map will be zoomed to the extent of either: <br/>
  a. Final path - address points to the safety location <br/>
  b. Entire study area <br/>
  Additionally, the view on the QGIS Map Canvas is also exported as an image in the output folder <br/>
![image](https://user-images.githubusercontent.com/80443493/137458386-f89b5f60-569c-443f-9f1a-78c0fbb5b4cd.png)

