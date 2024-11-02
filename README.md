# Intelligent-DoS-and-DDoS-Detection-A-Hybrid-GRU-NTM-Approach-to-Network-Security

**Author:** Caroline Panggabean; Chandrasekar Venkatachalam; Priyanka Shah; Sincy John; P Renuka Devi; Shanmugavalli Venkatachalam  
**Published in:** [2024 5th International Conference on Smart Electronics and Communication (ICOSEC), 2024]  
**Link to Paper:** https://ieeexplore.ieee.org/document/10722438

---

## Overview

This repository contains the code for the research paper titled "Intelligent DoS and DDoS Detection: A Hybrid GRU-NTM Approach to Network Security," which presents a hybrid deep learning model combining Gated Recurrent Units (GRU) and Neural Turing Machine (NTM) layers for enhanced intrusion detection in cybersecurity. This model was tested on UNSW-NB15 and BoT-IoT datasets, achieving a 99% accuracy rate in distinguishing between normal, DoS, and DDoS traffic, which marks a significant advancement in real-time threat detection.

---

## Requirements

To install the dependencies, you can use:

```bash
pip install -r requirements.txt
```

## Getting Started
Clone the Repository:
```bash
git clone https://github.com/olinexs/Intelligent-DoS-and-DDoS-Detection-A-Hybrid-GRU-NTM-Approach-to-Network-Security.git
```

## Project Structure
- code.ipynb: Contains the full implementation of the hybrid GRU-NTM model for DoS and DDoS detection.
- data/ (optional): Folder for datasets or a link to download them if needed.
- requirements.txt: List of libraries required to run the notebook.

## Data Collection and Preprocessing
This model uses the following datasets:
- UNSW Normal Traffic Dataset: Includes typical network traffic data.
- BoT-IoT DoS Dataset: Contains data from simulated DoS attacks in an IoT environment.
- BoT-IoT DDoS Dataset: Contains data from simulated DDoS attacks.
Each dataset undergoes data balancing, normalization, and encoding, as outlined in the notebook

## Model Architecture
The model consists of:

* GRU Layers: For processing sequential data and short-term dependencies.
* Neural Turing Machine (NTM): Provides long-term memory and enables the model to reference past information, crucial for complex pattern detection.
* Dense Layers: For further feature abstraction.
* Output Layer: SoftMax layer with three classes (Normal, DoS, DDoS).
