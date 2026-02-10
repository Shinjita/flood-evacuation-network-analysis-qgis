# Flood Evacuation Network Analysis using QGIS Python

This project presents an **automated GIS-based network analysis workflow** developed in **QGIS using Python**, designed to identify **safe evacuation routes during flood events**. The tool integrates spatial data, network analysis, and cartographic styling to support rapid decision-making in emergency and disaster response contexts.
The workflow focuses on identifying the **fastest or shortest evacuation paths** from flood-affected residential addresses to designated **safety points** (e.g. schools, shelters), while accounting for flood extents, buffer zones, and road network constraints.

## Project Purpose

Flood events require **rapid, repeatable, and reliable evacuation planning**. Manual GIS workflows are often too slow and error-prone during emergencies. This project demonstrates how **GIS automation** can be use to an **applied urban risk and resilience analysis**, suitable for emergency management, urban planning, and spatial decision-support systems.

## What This Project Does
At a high level, the workflow:

1. Identifies flood-affected areas using buffered flood polygons  
2. Selects a user-defined safety point (by name or coordinates)  
3. Clips road networks and address points to the affected study area  
4. Determines which addresses are closest to the selected safety point  
5. Computes the **shortest or fastest evacuation routes** using network analysis  
6. Applies predefined cartographic styles for clear visual interpretation  
7. Outputs both map layers and an exported map image for reporting  

## How to Run the Code
### Prerequisites
- QGIS (with Python support enabled)
  
### Step 1: Load the Main Script
Open QGIS, launch the Python Console, and load the `code.py` script. This will register the custom **Network Analysis: Safety Point Identification** tool in the QGIS Processing Toolbox.<br/>
![image](https://user-images.githubusercontent.com/80443493/137457987-38bdd4da-ce5e-4514-8abe-0661a9cf565b.png)

### Step 2: Run the Processing Tool
From the Processing Toolbox, run **Network Analysis: Safety Point Identification** and provide the required inputs, including flood buffer distance, selected safety point name, safety point coordinates, input spatial layers, and optional QML symbology files.<br/>
![image](https://user-images.githubusercontent.com/80443493/137458045-f55cde87-6888-4749-b781-664f4e4d6079.png)

### Step 3: Review the Output Layers
From the Processing Toolbox, run **Network Analysis: Safety Point Identification** and provide the required inputs, including flood buffer distance, selected safety point name, safety point coordinates, input spatial layers, and optional QML symbology files.<br/>
![image](https://user-images.githubusercontent.com/80443493/137458213-41af22e8-dfb5-4f3f-88ab-f726765e1cfa.png)

### Step 4: Export the Map Output
Run the `export_image_code.py` script from the Python Console to automatically zoom to the final evacuation route or study area and export the map view as an image to the output folder.<br/>
![image](https://user-images.githubusercontent.com/80443493/137458312-9fb413d9-c716-40bf-af63-7589e1802d66.png)

### Step 5: Re-run for Different Scenarios
The workflow can be re-run with different buffer distances, safety points, or study areas to support rapid evacuation scenario testing.<br/>
![image](https://user-images.githubusercontent.com/80443493/137458386-f89b5f60-569c-443f-9f1a-78c0fbb5b4cd.png)

