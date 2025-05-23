# WebAppKPI
This web app is an application for monitoring and comparing the performance of two machine learning models applied to the MNIST dataset: a centralized model (CNN) and a federated model (FedAvg). Below is a detailed description of its main components:

1.Application Structure:

   - Backend: Developed with Flask (app.py)
    
   - Frontend: HTML, CSS, and JavaScript with Chart.js for visualization
    
   - Data Management: Structured data stored directly in the backend

2.Main Pages:

  2.1Home Page (index.html):

   - Displays information about the MNIST dataset
    
   - Shows an overview of the models' performance
    
   - Links to model details and comparison page

2.2 Model Detail Page (model_detail.html):

   - Displays detailed information about a single model
    
  -  Shows specific KPI metrics:
    
     - Accuracy
      
     - Loss
      
     - Execution time
      
     - Memory usage
      
     - Instruction count

2.3 Comparison Page (compare.html):

  - Compares the performance of the two models through:
  
    - Line chart for accuracy
    
    - Bar chart for resource usage
    
   -  Radar chart for multidimensional comparison
    
   - Detailed metrics table

3 Visualizations (charts.js):

  -Interactive charts created with Chart.js:
  
     - Line chart for accuracy progression
      
     - Bar chart for comparing normalized metrics
      
     - Radar chart for multidimensional performance visualization
      
     - Gauge chart for specific metrics

4. Style and Design (style.css):

 - Responsive design to adapt to different screen sizes
  
-  Grid layout for metrics
  
 - Cards for organizing information
  
 - Font Awesome icons for enhanced user experience

5. API Functionality:

- Endpoints to retrieve model data (/api/models)
 
- Endpoints to update model metrics (/api/update_model)
 
- Data managed in memory for optimal performance

The application is designed to provide a clear and comparative view of the performance of the two machine learning approaches (centralized vs. federated) on the MNIST dataset, with a particular focus on visualizing key performance metrics.

#Guide to Running Web Application

-Prerequisites:
pip install flask
-Starting the Application:
python app.py
