# Project Title:  
**Road Type Classification for GNSS Toll System**

## Description:
Road Type Classification is crucial in GNSS-based toll systems for calculating toll or usage costs. The cost of using a service road is significantly lower than that of a highway, and this project focuses on classifying road types to determine toll charges accurately.

The classification is based on GNSS data, including latitude, longitude, speed, heading (degrees), and altitude. The **heading** is the primary feature for classification, as service roads typically involve more turns, with heading values lower or higher than 90 degrees. In contrast, highways involve straight movements, where the heading remains around 90 degrees.

The data used for classification is GNSS data gathered from satellites.

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

## Technologies used:

- **Programming language**: Python
- **Libraries used**: Pandas and scikit-learn
