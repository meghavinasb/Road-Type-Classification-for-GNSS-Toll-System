# Project Title:  
**Road Type Classification for GNSS Toll System**

## Description:
Road Type Classification is crucial in GNSS-based toll systems for calculating toll or usage costs. The cost of using a service road is significantly lower than that of a highway, and this project focuses on classifying road types to determine toll charges accurately.

The classification is based on GNSS data, including latitude, longitude, speed, heading (degrees), and altitude. The **heading** is the primary feature for classification, as service roads typically involve more turns, with heading values lower or higher than 90 degrees. In contrast, highways involve straight movements, where the heading remains around 90 degrees.

The data used for classification is GNSS data gathered from satellites.

This project classifies roads into two categories: **Highway** and **Service Road** using a machine learning model trained on a synthetic dataset. The goal is to assist in various GNSS (Global Navigation Satellite System) applications where road type information is crucial for route planning, autonomous driving, and safety.

## Motivation/Background:

### 1. **Infrastructure Cost Reduction**
- **Traditional Tolling**: Expensive infrastructure like toll plazas, cameras, and barriers is needed, and maintaining this can be costly.
- **GNSS Tolling**: No physical infrastructure is required. Vehicles calculate tolls automatically based on location, reducing costs significantly.

### 2. **Scalability & Flexibility**
- **Traditional Tolling**: Limited to specific locations, requiring new infrastructure for expansion.
- **GNSS Tolling**: Highly flexible and scalable. Authorities can adjust tolling zones, and implement pricing based on time, region, or road quality, without adding new hardware.

### 3. **Congestion Management**
- **Traditional Tolling**: Causes congestion at toll points as vehicles must stop or slow down.
- **GNSS Tolling**: No need to stop, allowing for free-flow traffic and reducing bottlenecks.

### 4. **Accuracy & Dynamic Pricing**
- **Traditional Tolling**: Charges are usually flat or distance-based per booth location.
- **GNSS Tolling**: Provides precise location-based tolling, enabling dynamic pricing models, such as time-of-day or congestion-based rates.

### 5. **Better Coverage & Tolling Fairness**
- **Traditional Tolling**: Misses road usage in certain areas, leading to unfair charging.
- **GNSS Tolling**: Tolls are calculated based on actual road usage, making it fairer for both short and long-distance drivers.

### 6. **Environmental Impact**
- **Traditional Tolling**: Stopping at toll points increases fuel consumption and emissions.
- **GNSS Tolling**: Improves fuel efficiency by reducing stop-and-go traffic, lowering emissions.

### 7. **No Manual Intervention**
- **Traditional Tolling**: May require manual transactions or systems like RFID.
- **GNSS Tolling**: Fully automated, reducing operational costs and human error.

### 8. **Cross-border Compatibility**
- **Traditional Tolling**: Limited to specific countries or regions.
- **GNSS Tolling**: Allows seamless tolling across regions and countries, using a single device or app.

### 9. **Data Collection & Analytics**
- **Traditional Tolling**: Limited data collection.
- **GNSS Tolling**: Provides rich traffic data, which can be used to improve traffic management and infrastructure planning.

### 10. **User Convenience**
- **Traditional Tolling**: Requires carrying cash or having accounts.
- **GNSS Tolling**: Automated deductions based on travel, providing a hassle-free experience.

### 11. **Pay for Exact Road Usage**
- **Traditional Tolling**: Drivers pay a fixed fee at toll booths, often overpaying for unused road sections.
- **GNSS Tolling**: Drivers are charged only for the exact distance they travel, ensuring fairness. This distance-based charging eliminates the issue of paying for road sections that aren't used.


## Key Features
- **Binary Road Classification**: Distinguishes between highways and service roads based on input data.
- **Model Performance**: Achieves **84.50%** accuracy, with detailed classification metrics provided.
- **Confusion Matrix**: Offers insight into misclassification patterns, helpful for model improvements.

## Performance Metrics
The machine learning model was trained and evaluated on a dataset of 200 samples. Below are the key metrics for model performance:

### Accuracy
- The overall accuracy of the model is **84.50%**, meaning it correctly classifies road types in 84.50% of the cases.

### Classification Report
|               | Precision | Recall  | F1-Score | Support |
|---------------|-----------|---------|----------|---------|
| **Highway**   | 0.76      | 1.00    | 0.86     | 98      |
| **Service Road**| 1.00      | 0.70    | 0.82     | 102     |
| **Accuracy**  |           |         | 0.84     | 200     |
| **Macro Avg** | 0.88      | 0.85    | 0.84     | 200     |
| **Weighted Avg** | 0.88      | 0.84    | 0.84     | 200     |

### Confusion Matrix
The confusion matrix below shows the correct and incorrect classifications:

- **98** true positives for highways (correctly classified as highways).
- **71** true positives for service roads (correctly classified as service roads).
- **31** false negatives for service roads (incorrectly classified as highways).
- **0** false positives for highways.

## Technologies used:

- **Programming language**: Python
- **Libraries used**: Pandas and scikit-learn

## Usage:
1. **Install Required Libraries**: Ensure that `pandas` is installed in your Python environment. You can install it via pip:
   ```bash
   pip install pandas
2. **Install Required Libraries**: Ensure that `scikit-learn` is installed in your Python environment. You can install it via pip:
   ```bash
   pip install scikit-learn

## Future Improvements
- Explore additional features and algorithms to enhance classification performance.
- Test the model on real-world datasets.
