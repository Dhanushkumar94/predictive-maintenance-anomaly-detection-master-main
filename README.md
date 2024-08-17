# Automated Anomaly Detection for Predictive Maintenance

Automated Anomaly Detection for Predictive Maintenance is a machine learning project focused on enhancing the efficiency of maintenance operations in industrial settings. By leveraging predictive maintenance techniques, the project aims to automate the detection of anomalies and potential equipment failures, allowing for proactive and timely interventions. The repository contains machine learning models, data preprocessing scripts, and visualization tools to streamline the predictive maintenance process and improve overall operational reliability.

# Motivation

In the realm of industrial operations, efficient maintenance plays a pivotal role in ensuring the continuous and smooth functioning of machinery. The motivation behind this project stems from the need to revolutionize traditional maintenance practices by incorporating cutting-edge technology.

Automated Anomaly Detection for Predictive Maintenance is driven by the desire to shift from reactive to proactive maintenance strategies. The aim is to harness the power of machine learning to predict potential equipment anomalies and failures before they occur. By doing so, the project seeks to minimize downtime, reduce maintenance costs, and enhance the overall reliability of industrial systems.

This initiative is motivated by the vision of creating a more resilient and optimized industrial landscape through the application of advanced data-driven methodologies. The project endeavors to contribute to the ongoing evolution of predictive maintenance, making it an integral part of smart and sustainable industrial practices.


# Visuals

Here are some snapshots showcasing different aspects of the Automated Anomaly Detection for Predictive Maintenance project. These visuals provide a glimpse into the functionality and user interface of the system.

1. **Dashboard Overview:**
   ![Dashboard Overview](/Visuals/EDA_Overview.jpeg)
   ![Dashboard Overview](/Visuals/variables.png)
   ![Dashboard Overview](/Visuals/interactions.png)
   ![Dashboard Overview](/Visuals/correlations.png)
   

3.  **Anomaly Detection Results:**
    ![Anomaly Detection Results](/Visuals/anomaly_results.jpeg)
    **Actual vs Predicted Scores for Validation Data:**
    This graph visualizes the comparison between the actual labels and the predicted scores generated by our anomaly detection model using 
    validation data.

    **True Label (Marker: o)**: The true labels represent the actual occurrence of anomalies in the validation dataset. Each point on the 
    graph corresponds to a specific example within the dataset.

    **Predicted Score (Marker: x)**: The predicted scores are the anomaly scores assigned by our model to each example in the validation 
    dataset. These scores indicate the likelihood of an anomaly being present, with higher scores suggesting a higher likelihood.

    By comparing the true labels with the predicted scores, we can assess how effectively our model identifies anomalies and understand its 
    performance across different examples.

4.  **Data Visualization:**
    ![Data Visualization](/Visuals/ROC_curve.jpeg)

    **ROC curve:**
    The Receiver Operating Characteristic (ROC) curve visualizes the performance of our anomaly detection model based on the true positive 
    rate (sensitivity) against the false positive rate (1 - specificity) across different threshold values.

    **ROC Curve (AUC = 0.91)**: The ROC curve illustrates the trade-off between true positive rate and false positive rate at various 
    threshold levels. A higher area under the curve (AUC) value indicates better discrimination ability of the model between normal and 
    anomalous instances.

    **Baseline Line (Diagonal dashed line)**: The diagonal line represents the baseline performance of a random classifier.

    By examining the ROC curve, we can assess the model's ability to distinguish between normal and anomalous instances, with a higher AUC 
    value indicating superior performance.

    ![Data Visualization](/Visuals/precision_Recall_curve.jpeg)

    **Precision-Recall Curve:**
    The Precision-Recall curve provides insights into the trade-off between precision and recall for our anomaly detection model.

    **Precision-Recall Curve (AUC = 0.85)**: The Precision-Recall curve illustrates the model's precision (positive predictive value) 
    against recall (sensitivity) across different threshold values. The area under the curve (AUC) reflects the model's ability to balance 
    precision and recall effectively.

    By analyzing the Precision-Recall curve, we can evaluate the model's performance in identifying anomalies while minimizing false 
    positives. A higher AUC value indicates superior precision-recall balance and model effectiveness.

    ![Data Visualization](/Visuals/confusion_matrix.jpeg)

    **Confusion Matrix:**
    The confusion matrix provides a comprehensive overview of the performance of our anomaly detection model by comparing predicted labels 
    with actual labels.

    **Heatmap Representation**: The heatmap visualizes the confusion matrix, where actual labels are displayed on the vertical axis and 
    predicted labels on the horizontal axis. Each cell in the matrix indicates the count of instances for a specific combination of 
    predicted and actual labels.

    **Interpretation**: Correct predictions are represented by cells along the diagonal, where the predicted label matches the actual 
    label. Off-diagonal cells signify misclassifications, highlighting areas where the model may be struggling to differentiate between 
    normal (0) and anomalous (1) instances.

    **Annotations**: The numbers within each cell denote the count of instances for the corresponding combination of predicted and actual 
    labels.

    By analyzing the confusion matrix, we gain valuable insights into the model's strengths and weaknesses, allowing us to refine and 
    improve its performance over time.

    ![Data Visualization](/Visuals/calibration_curve.jpeg)

    **Calibration Curve:**
    The calibration curve provides insights into the calibration of our anomaly detection model by comparing the mean predicted 
    probabilities with the actual fraction of positives across different probability thresholds.

    **Curve Representation:** The curve visualizes the relationship between the mean predicted probabilities and the fraction of positive 
    instances. Each point on the curve represents a probability threshold, with the x-axis indicating the mean predicted probability and 
    the y-axis representing the fraction of positive instances.

    **Perfectly Calibrated Line:** The dashed gray line represents perfect calibration, where the predicted probabilities perfectly match 
    the actual fraction of positives. Deviations from this line indicate potential calibration errors or discrepancies in the model's 
    probability estimates.

    By analyzing the calibration curve, we can assess the reliability and accuracy of our model's predicted probabilities and identify 
    areas for calibration refinement.

# Features

Automated Anomaly Detection for Predictive Maintenance comes packed with a range of powerful features, making it a standout solution in the field. Here are some key highlights:

1. **Predictive Maintenance Models:**
   - The project includes robust machine learning models designed for predictive maintenance, helping anticipate equipment failures before 
     they occur.

2. **Real-time Anomaly Detection:**
   - The system provides real-time anomaly detection, allowing for immediate response to potential issues as they arise.

3. **Visualization of Anomalies:**
   - Matplotlib and Seaborn are utilized to generate visualizations that aid in understanding and interpreting anomalies detected by the 
     models.


These features collectively make Automated Anomaly Detection for Predictive Maintenance a comprehensive and effective solution for ensuring equipment reliability and minimizing downtime.


# How to Use?

The explanation of every step is also given in the Jupyter Notebook <a href="Notebooks/Anoma.ipynb" target="_blank">Anoma.ipynb</a> and you can also check the <a href="/Anoma_report.pdf" target="_blank">Anoma_report.pdf</a> for the same.

Follow these steps to effectively use the Automated Anomaly Detection for Predictive Maintenance project:

**Clone the Repository:**

Clone this repository to your local machine using the following command:

git clone https://github.com/Dhanushkumar94/predictive-maintenance-anomaly-detection-master.git

**Install Dependencies:**

Navigate to the project directory:
cd predictive-maintenance-anomaly-detection/Notebooks

Install the required Python dependencies using:
pip install -r requirements.txt

**Open the Jupyter Notebook:**

Launch Jupyter Notebook:

Open the Anoma.ipynb notebook.

**Run the Notebook Cells:**

Execute each cell in the notebook sequentially.
Pay attention to the comments and markdown cells for guidance on each step.

**Explore the Results:**

Analyze the visualizations and insights provided by the notebook.
Customize parameters or experiment with your own datasets if needed.

**Model Deployment (Optional):**

Deploy the trained model for real-time anomaly detection, refer to the deployment section in the notebook for guidelines.

**Real-time Anomaly Detection and Visualization of Anomalies:**
Make inferences, visualize Anomalies, prediction results, Evaluation, and Deeper Insights by creating a predictor instance using the endpoint name of the deployed model, refer to the Cross Evaluation and Deeper Insights section in the notebook


## Feedback:

Provide feedback or report issues through GitHub.

By following these steps, you can effectively utilize the anomaly detection capabilities of the project for predictive maintenance in your own datasets.


# Credits
I would like to express our gratitude to the following resources that have been instrumental in the development of Automated Anomaly Detection for Predictive Maintenance:

 **XGBoost**:

The project utilizes the powerful XGBoost library for predictive modeling. XGBoost GitHub Repository

**Scikit-learn:**

Leveraging Scikit-learn for various machine learning utilities. Scikit-learn GitHub Repository

**GitHub:**

Valuable insights and inspiration from various open source projects on GitHub.

**Data Science Community:**

Continuous learning and inspiration from the vibrant data science and machine learning communities.

**Online Resources:**

AWS Documentation, Blogs, articles and tutorials that provided valuable insights and knowledge.
I appreciate the collective efforts of the open-source community and the wealth of knowledge shared by individuals and organizations.

If you find any resource missing or would like to be credited, please let us know, and I'll make sure to acknowledge your contributions.

Thank you for being part of this journey!

**Dhanush Kumar ** - **Data Scientist**


