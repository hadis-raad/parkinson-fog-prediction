## Predicting Parkinson's Freezing of Gait Episodes: A Comprehensive Step-by-Step Approach¶
Freezing of gait (FOG) is a debilitating symptom that affects individuals diagnosed with Parkinson’s disease, which significantly impacting their ability to walk and limiting their mobility and independence. Machine learning (ML) techniques can provide valuable insights into the occurrence and causes of FOG episodes. By leveraging ML, medical professionals can enhance their evaluation, monitoring, and prevention of FOG events.

This notebook is based on [Parkinson's Freezing of Gait Prediction competition dataset on kaggle](https://www.kaggle.com/competitions/tlvmc-parkinsons-freezing-gait-prediction) which includes data collected from a wearable 3D lower back sensor. The goal of this project is detecting the start and stop of each freezing episode, as well as identifying three types of FOG events: Start Hesitation, Turn, and Walking.

A lower-back 3D accelerometer captures the following features related to FOG detection:

* AccV: acceleration measured by a vertical sensor
* AccML: acceleration measured by a mediolateral sensor
* AccAP: acceleration measured by an anteroposterior sensor
<div style="text-align: center;">
  <img src="https://github.com/hadis-raad/parkinson-fog-prediction/blob/main/axis%20of%20movement.png" alt="axis of movement" width="400"/>
</div>

After collecting data, necessary preprocessing steps, such as handeling missing data, handling categorical variables, data normalization, and outlier detection, were performed on the dataset. In this multi-class classification project, where the mean average precision is the evaluation metric, various ML algorithms were tuned. Ultimately, the LightGBM algorithm was chosen as the model for further analysis.
