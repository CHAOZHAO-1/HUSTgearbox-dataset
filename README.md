# HUSTgearbox dataset (实验室自采开源数据集，包含稳定转速和时变转速)

**Important updata 2024-05-19. The second column of the file represents speed. However, since we collected the data at a constant speed, this column is redundant and holds no meaningful value. You can ignore it. The correct speed is indicated in the filename.**

We released an open-source gearbox failure dataset. 

We hope this dataset can benefit your research


data of Google Drive: https://drive.google.com/drive/folders/1Lt8Xu6NICPadliXhOtDMB683uKwZv4FP?usp=sharing


## Dataset overview

This dataset comprises vibration signals from gearbox in **3** different health states under **30** distinct operating conditions.

These datasets are publicly available, and anyone can use them to validate diagnosis algorithms for gearbox. Publications making use of the HUSTgearbox datasets are requested to cite the following paper.

**Chao Zhao, Enrico Zio, Weiming Shen, Domain Generalization for Cross-Domain Fault Diagnosis: an Application-oriented Perspective and a Benchmark Study, Reliability Engineering and System Safety (2024), doi: https://doi.org/10.1016/j.ress.2024.109964.**

 ![image](https://github.com/CHAOZHAO-1/HUSTgearbox-dataset/blob/main/IMG/F1.png)
 
Fig. 1. (a) Test rig of HUSTgearbox dataset.

## Brief introduction to experiments

### Gearbox testbed
The gearbox fault tests were conducted using a Spectra-Quest Mechanical Fault Simulator, as depicted in Fig. 1.

From left to right on the test rig are speed control, motor, acceleration sensor, gearbox, and data acquisition board. 

The gearbox in three health states is illustrated in Fig. 2,   

(1) Normal,   

(2) Broken tooth,  

(3) Missing tooth.  

It’s important to note that all faults are artificially preset.

![image](https://github.com/CHAOZHAO-1/HUSTgearbox-dataset/blob/main/IMG/F2.png)

Fig. 2. Photographs of the failure gears.
 

### Tested gearbox
Fig. 3 display the tested gearbox, and its details are listed as following:

Ratio: 1.5:1

Gearbox Model: Hub City M2

Pitch Angle Gear: 56°19’

Pitch Angle Pinion: 33° 41’

Pressure Angle for Gear and Pinion: 20°

Material: Forged steel

Backlash tolerance: 0.001-0.005 inches

Pitch diameter pinion: 1.125 inches

Pitch diameter gear: 1.6875 inches

Number teeth pinion: 18

Number teeth gear: 27

Pinion bearing: NSK 6202 (1 bearing)

Gear bearing: (2 bearings)

### Operating Condition

A total of 30 different operating conditions (5 types of loads and 6 types of speeds) were set in experiments.   

The operating load include:  
1)	0 Nm  
2)	0.113 Nm  
3)	0.226 Nm  
4)	0.339 Nm  
5)	0.452 Nm
   
The operating speed include:  
1)	20 Hz   
2)	25 Hz   
3)	30 Hz   
4)	35 Hz   
5)	40 Hz  
6)	0-40-0 Hz,   see Fig. 3.

![image](https://github.com/CHAOZHAO-1/HUSTgearbox-dataset/blob/main/IMG/F3.png)

Fig. 3. Time-varying speed.

   
The rotating speed is adjusted by the speed control, and the load is regulated by the load control device. 


### Sampling setting

The sampling frequency is set to 25.6 kHz.

A total of 262144 data points (i.e. 10.2s) are recorded for each sampling.
 


## Dataset details
The raw data file comprises 90 files (3 health states multiplied by 30 working conditions), each in TEXT format.

For instance, the filename " B_20_1 " indicates broken tooth fault under the 20 Hz and 1×0.113 Nm working condition.

The health states are represented by the following codes:

H: Healthy

B: Broken tooth

M: Missing tooth

## Contact

If you have any questions or suggestions, do not hesitate to contact: 

Mr. Chao Zhao, zhaochao734@hust.edu.cn

