# Smart Gym System

## Overview  
The Smart Gym System is a context-aware fitness guidance solution that leverages real-time data from sensors, exercise equipment, and probabilistic models to enhance the user’s workout experience. The system consists of:  
1. **Protégé Ontology** - Represents the knowledge base for fitness recommendations.  
2. **Netica Bayesian Models** - Models decision-making scenarios for gym crowd management, workout progression, and nutrition guidance.  

---

## Protégé Ontology

### **Description**  
The **smartGym.rdf** file defines the ontology of the Smart Gym System, structuring knowledge about fitness routines, user profiles, health conditions, and equipment. It allows semantic reasoning to provide personalized workout recommendations.  

### **Key Components**  
- **Users**: Categorized based on fitness level (beginner, athlete, elderly, rehab patient).  
- **Exercise Equipment**: Treadmills, weight machines, and smart devices.  
- **Health Metrics**: Age, BMI, heart rate, and calories burned.  
- **Workout Plans**: Personalized routines based on real-time feedback.  
- **Sensors**: Smartwatches, RFID readers, and embedded exercise sensors.  

### **Usage**  
1. Open **Protégé** and load the `smartGym.rdf` file.  
2. Use reasoners (e.g., Pellet) to infer user-specific recommendations.  
3. Query the ontology using SPARQL to retrieve customized workout plans.  

---

## Netica Bayesian Models  

### **Description**  
Three Bayesian networks model the decision-making process in a smart gym using probabilistic reasoning.  

### **Files**  
1. **GYM.neta** - Manages gym crowd levels and suggests whether to wait, work out, or leave.  
2. **GYM2.neta** - Tracks workout task progression based on calories burned and heart rate.  
3. **GYM3.neta** - Suggests post-workout nutrition based on the user’s health profile.  

### **Usage**  
1. Open **Netica** and load the `.neta` files.  
2. Input real-time data (crowd status, workout performance, health data).  
3. Run inference to receive personalized recommendations.  
