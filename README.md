<h1>Short-Term Solar Irradiance Forecasting for Energy-Efficient Infrastructure: A Deep Learning Case Study of Delhi</h1>
Authors: Himanshi Kaura¹, Hardeep Kaur² <br>
Affiliation: Guru Nanak Dev University

## Project Overview
This study contributes to the development of **robust and scalable solar irradiance forecasting systems**, which are essential for optimized scheduling and sustainable energy management in smart grids.
We propose and implement four deep learning architectures:
- **Deep Regularized LSTM (DR-LSTM)**
- **GRU with Attention Mechanism (GRAtt)**
- **Temporal Informer (T-Informer)**
- **Temporal Self-Attention Transformer (T-SAT)**

To train and evaluate these models, we use hourly satellite-based meteorological data collected between **January 1, 2020, and July 31, 2024**.

## Dataset
<ul>
<li>Source: NASA POWER API</li>
<li>Location: Delhi, India (28.7041°N, 77.1025°E)</li>
<li>Duration: Jan 1, 2020 – July 31, 2024</li>
<li><ul>Features:
  <li>Solar Irradiance (ALLSKY_SFC_SW_DWN)</li>
  <li>Temperature (T2M)</li>
  <li>Cloud Cover (CLOUD_AMT)</li>
  <li>Relative Humidity (RH2M)</li>
  <li>Hour, Day, Season (encoded)</li></li></ul>

The cleaned dataset is saved as a `.csv` file and resides in the same folder as the main script.

Our methodology follows a systematic pipeline:
- **Data preprocessing**
- **Temporal sequencing** using a **sliding window technique**
- **Model development, training, and evaluation**
These models aim to capture complex temporal patterns in atmospheric data, contributing to accurate short-term solar forecasting.
---

## Requirements
numpy==1.24.4               
pandas==1.4.4                  
matplotlib==3.5.2              
seaborn==0.11.2                
scikit-learn==1.0.2              
tensorflow==2.12.0               
keras==2.12.0                   
torch==2.6.0                    
transformers==4.27.4       

## Clone This Repository
To get a local copy of this project on your machine, run the following command in your terminal:

```bash
git clone https://github.com/Himanshikaura/solar-irradiance.git
```
## Credits
This project was developed as part of an academic exploration in solar forecasting and deep learning. Special thanks to open-source contributors and libraries used in this project.

## License
This repository is open-sourced under the MIT License.
