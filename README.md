 #  TornadoTracker🌪️
> The TornadoTracker App is designed to revolutionize how individuals receive tornado warnings. By leveraging the capabilities of machine learning with the AlexNet convolutional neural network, the app offers precise and timely tornado detection. Its primary aim is to analyze live weather radar images, identify potential tornado formations, and provide immediate, localized alerts. This proactive approach aims to enhance safety during severe weather conditions, especially during the night when the risk of undetected tornadoes is greatest. The TornadoTracker App is about empowering users with advanced warning, maximizing preparedness and response time for communities worldwide.

<div align="center"> <img src="https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/Tornadotrackerlogo.png"> </div>

&ensp;

## 🚨 Tornado Detection Challenge
> Tornadoes pose a significant threat to safety, especially when they strike unexpectedly. Current systems for tornado detection and warning are often inadequate, leading to delayed responses and increased risk, particularly at night. Our app aims to address these challenges head-on, offering a more effective solution.

- **Limited Localized Warnings:** 
  - Current severe weather forecasting systems provide broad area warnings, lacking precision for localized tornado paths.
  - General alerts cover large areas, failing to pinpoint specific neighborhoods or streets at risk.
- **Night Time Tornadoes:** 
  - Higher casualty and injury rates at night due to decreased visibility and lower public awareness.
  - Many people are asleep and miss warnings, increasing the risk of harm.
- **Lack of Expertise Among the Public:** 
  - Most individuals lack the skills to accurately interpret weather radar imagery.
  - This lack of knowledge leads to delayed or missed responses during critical moments.
- **Global Applicability:** 
  - Numerous regions worldwide are devoid of advanced weather reporting systems.
  - These areas, however, often have access to live radar images but lack the means to analyze and communicate warnings effectively.
&ensp;
 <div align="center"> <img src="https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/Storm-relative-velocity%20radar-images.png"> </div>
 
 &ensp;

## 👨‍👩‍👦‍👦 Empowering Communities with Advanced Detection
> In the face of natural disasters like tornadoes, timely and accurate information is crucial. Our product, TornadoTracker, leverages advanced technology to provide real-time, localized tornado warnings, making safety more accessible to everyone, everywhere.

- **Real-Time, Precise Alerts:** 
  - Deliver immediate, pinpointed tornado warnings to users' smartphones.
  - Significantly improves response time and safety in affected areas.
- **Enhanced Night Time Safety:** 
  - Special focus on nighttime detection to mitigate the higher risk of casualties.
  - Critical alerts can wake users and provide them with life-saving information.
- **Global Reach and Application:** 
  - Ideal for regions lacking sophisticated weather forecasting systems.
  - Can leverage existing radar data to provide advanced warnings where none were previously available.
 &ensp;
 <div align="center"> <img src="https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/tornadotrackermockup%20(1).gif""> </div>   

&ensp;

## 🤖 Our Solution Using AlexNet: Leveraging Machine Learning for Enhanced Safety
> By utilizing AlexNet, a convolutional neural network, we can classify live weather radar images with high accuracy, enhancing safety and response times in tornado-prone areas.

- **Model Overview:** 
  - AlexNet, a proven convolutional neural network, classifies live weather radar images.
  - Categorizes images into two distinct groups: tornado and no-tornado.
- **Data Processing and Training:** 
  - Model trained on a curated dataset.
  - Focuses particularly on identifying the unique signatures of tornadoes.
- **Advanced Feature Extraction:** 
  - AlexNet's layers are adept at capturing complex patterns.
  - These capabilities are crucial for distinguishing tornadoes from other weather phenomena.
- **Real-Time Analysis and Response:** 
  - The app analyzes live radar feeds continuously, using the trained model for instant detection.
  - Ensures timely and accurate alerts to users in potential tornado paths.
- **Visual Insights Through Feature Maps:** 
  - AlexNet provides feature maps, offering a window into what the model prioritizes in predictions.
  - These visualizations aid in understanding and improving model performance.

&ensp;
## 📈 TornadoTracker Model Analysis:

> **Accuracy - What It Measures:** Accuracy indicates how often our model correctly identifies tornadoes and thunderstorms in radar images.
> 
> - **Importance:** High accuracy is crucial for reliable predictions, ensuring that our system effectively warns of severe weather conditions.
>   
> **Loss - What It Measures:** Loss quantifies the error between the model's predictions and the actual labels in our training data.
> 
> - **Role in Improvement:** By minimizing loss, we refine the model's ability to detect complex weather patterns accurately, reducing false alarms and missed detections.
> 
> Monitoring these metrics helps us continuously improve our model, striving for a balance between high accuracy and low loss for dependable tornado detection.

 ### **Performance Summary:**
  - Accuracy:	93.2%
  - Loss: 0.42

---


![accplot](https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/tornadotracker-trainacc-plot.png)

![lossplot](https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/tornadotracker-loss.png)


---
### **Feature Map Comparisons**
> Feature maps are the outputs of various layers within AlexNet. They represent how the network processes and identifies patterns in the input images. Initially capturing basic features like edges and colors, they progressively reveal more complex patterns in deeper layers.
> 
> **Application in Tornado Detection**
> 
> - **Pattern Recognition:** Feature maps help AlexNet identify specific signatures in radar images that are indicative of tornadoes and thunderstorms. This includes recognizing unique shapes, intensities, and movements often associated with severe weather conditions.
> 
> - **Enhancing Accuracy:** By analyzing these maps, we can understand and improve how the network distinguishes between normal weather patterns and potential severe weather threats, enhancing the accuracy and reliability of our tornado detection system.

&ensp;

### High-Response Filters: Unveiling Key Features in Storm Detection
High-response filters in our neural network play a pivotal role in analyzing storm relative velocity radar images. These filters are highly reactive to certain features in the data, providing valuable insights into the distinguishing characteristics of tornadoes and thunderstorms.

- **Identifying Contrast and Defining Features:**
  Our analysis revealed that both tornadoes and thunderstorms elicit strong responses from specific filters, particularly in areas of high contrast. This characteristic is crucial as it highlights the most defining features of these weather phenomena, accentuating their differences and their possible similarities


![highres-filterdemo](https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/HighRes-Filters-Demo.gif)

&ensp;

### Low-Response Filters: Capturing Subtle Distinctions
On the other hand, the low-response filters are less sensitive but equally important. They often reveal subtle, yet critical, details that high-response filters might overlook.

- **Revealing Finer Details:**
  These filters may show weaker responses, indicating fewer similarities between the filter pattern and the image. However, this subtlety is key to uncovering less obvious features that distinguish tornadoes from thunderstorms.
- **Detecting Motion and Subtle Changes:**
  In particular, the low-response filters were more adept at picking up nuanced aspects like motion, which can be inferred from curvature and color changes in storm relative velocity radar images. These features, though less conspicuous than high-contrast areas, are vital for a comprehensive understanding of storm dynamics.



![lowres-filterdemo](https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/LowRes-Filters-Demo.gif)

---
<details>
  <summary><h3><strong> 📁 Access Our Report, Dataset, Feature Map Demos & Model: </strong></h3></summary>

  - [TornadoTracker Dataset](https://docs.google.com/presentation/d/1LDDAGeMAI8bAQunT5-fR2RQIVdAEHhksmrewBhtb1_g/edit?usp=sharing)
  - [TorndaoTracker Model Notebook](https://colab.research.google.com/drive/1cv4eTbLzWr-qSuYILD3vsRIQsQOUg6Pd#scrollTo=MJjTOJXQY7L2)
  - [TornadoTracker Feature Maps(Tornado)](https://colab.research.google.com/drive/1o178C_CcihPKepytHL9mtu-npnC_PWgs#scrollTo=pTdwBSAnfFlx)
  - [TornadoTracker Feature Maps(Thunderstorm)](https://colab.research.google.com/drive/17lBMJOVb6dqtNu20_mx441C-cHlPAXy2#scrollTo=pTdwBSAnfFlx)
  - [Project Report](https://github.com/cam-alvarez/tornado-tracker/blob/main/assets/TornadoTracker_Report.pdf)
</details>
