# Room Occupancy Estimation Using Sensor Data  
## Overview    

*Goal Of The Project:* 

  The primary goal of this project is to predict room occupancy levels (0,1,2,3) using environmental and motional sensors. By analyzing sensor data such as CO2 levels, PIR, sound, light and temperature. The model can estimate how many people are present at room in given time. This predictions helps in:  
* Optimizing energy consuption  
* Enhancing space utilization  
* Improving smart building automation
* Monitoring safety and crowd control

## Dataset  
* Source: UC Irvine Machine Learning Repository  
* Format: CSV  
* Instance: 10.13k  
* Features: 18 

## Features Used  
* **S5_CO2**:CO2 Concentration  
* **S5_CO2_Slope**: Rate of CO2 change  
* **PIR Sensors(S6,S7)**: Motion detection  
* **Average Temperature**: Combined average of all temperature sensors  
* **Average Light**: Combined average of all light sensors  
* **Average Sound**: Combined average of all sound sensors  
* **Hour,Day of week,Weekend**: Extracted from timestamp  

## Preprocessing Steps
* Removed redundant sensor columns  
* Engineered average features  
* Extracted datetime-based features  
* Label encoded terget classes  

## Model Used  
**Random Forest Classifier**  
   * Criterion: Gini  
   * Max Depth: 3 
   * Accuracy score: 98.6%  
   * Achieved good classification matrix and accuracy score  
      
## Visualizations  
* Feature importance visualized    
* Correlation Heatmap   
* Room Occupancy vs Day of Week   
* Confusion Matrix
  
## Conclusion  
The Room Occupancy Estimation project successfully demonstrates how environmental and motion sensor data can be used to predict the number of people present in a room using machine learning models.  

The following key point where observed: 
* Motion sensor (PIR) and CO2 levels showed strong correlation with occupancy.
* The Random Forest Classifier achieved high accuracy (98.6%) in predicting occupancy levels(0 to 3), making it the most effective model for this task.
* A clear pattern was observed: Rooms are typically occupied between 10:00 and 20:00 on Wednesdays, Fridays and Saturdays.
##  Tools Used  
* Python  
* Jupyter notebook  
* Pandas, NumPy  
* Scikit-Learn  
* Matplotlib, Seaborn  
## Author 
Hamda jubin    
Data science and Machine learning student   
email id: hamdack1994@gmail.com





   
   
   
  
 


