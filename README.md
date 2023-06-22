# STCIoT
Contains Dataset for Short Term Course

# Description Of Anomaly detection dataset
Most machine learning (ML) proposals in the Internet of Things (IoT) space are designed and evaluated on pre-processed datasets, where the data acquisition and cleaning steps are often considered a black box. Therefore, the data acquisition stage requires additional data cleaning/anomaly techniques, which translate to additional resources, energy, and storage. We propose to carry out such techniques not in the cloud servers and closer to the data source, on the IoT device itself. Consequently, this application defines three anomaly detection steps using smoothing filters, unsupervised learning, and deep learning techniques (hybrid model) to detect the different variations of anomalies, focusing on a small computational/memory footprint.

DATASET: 
To explain tamper situations, a test box was built to collect data from three different scenarios. The test box is made with a computer fan to cool the box, an incandescent bulb to warm up the box, and a small door that people can smoke or blow over the sensor. Therefore, label 1 is considered when the box is warming/cooling in normal conditions, label 2 when the sensor is tampered with by people blowing on it, label 3 is defined when people smoke near the sensor, and label 4 when the sensor detects fire. The IoT device has a well-known CO2, temperature, and humidity sensor SCD-30, the LoPy4 as a microcontroller and a relay board to manage the fan and the bulb. 

BACKGROUND:
Noise: The sensor's signal is discretized/digitalized to be understandable to the microcontroller. However, errors like voltage fluctuations, non-linearity response, and vibrations insert noise into the electric signal, confusing the ML algorithm in the feature extraction stage. For this reason, signal smoothing is a filter that reduces these noise components when the phenomenon does not have high sampling frequencies getting a cleaner signal.

Outlier detection: These methods are in charge of detecting data with a different distribution than the rest. This process is carried out through an unsupervised analysis.

Tamper detection: In some scenarios, the information acquired by the IoT device can be compromised by malicious users trying to steal or modify data. tamper detection techniques require knowing all the manipulation possibilities to detect them, which needs supervised learning.

# NF-Ton-IoT-v2
NF-ToN-IoT-V2 is the extended NetFlow version of NF-ToN-IoT. Compared to the original NF-NIDS datasets, the feature set of NetFlow features has expanded from 8 to 43.

This is one dataset in the NFV2-collection by the university of Queensland aimed at standardizing network-security datasets to achieve interoperability and larger analyses.

# Dataset Final csv file for Anomaly Detection
Grove sensors:

Grove - Temperature&Humidity Sensor (High-Accuracy &Mini) v1.0
Grove - Light Sensor
Grove - Loudness Sensor
Grove - Air Quality Sensor v1.3
Digi XBee 3 Zigbee 3 RF Module
Grove - UART Wifi V2
Microcontollers:

Arduino Nano 33 BLE Sense
Raspberry Pi Pico
Arduino Nano RP2040 Connect
Shields:

Grove - Bee Socket
Grove Shield for Pi Pico V1.0
Arduino Tiny Machine Learning Shield
Single-board computer:

Raspberry Pi 4 Model B
Software tools:

Putty
Raspberry Pi Imager
Node-RED
Arduino IDE 1.8.15
Visual Studio Code
Google Colab
How to generate a dataset via Grove sensors and Arduino is explained here.

We created anomalies at the following time intervals:

18:21:46 - 19:37:16 (first day)
02:26:36 - 04:15:56 (second day)
08:54:46 - 10:45:36 (second day)
