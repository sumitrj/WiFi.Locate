# WiFi.Locate

## Indoor Positioning System:
GPS or Global positioning systems are widely used to pin-point location of considered hardware in the global coordinate system.
Although huge number of satellites are used to accompalish this and these systems continue to imrove accuracy, they are not accurate when precision of distance less than 10m is intended.

## Problem Considered:
The places which demand precision of less than 10m are generally indoor environments. A subset of these environments include our own homes, wearhouses and precision robotics.

WiFi based location systems have been tested in various environments. The use of Ultrawideband waves to make an indoor positioning system has exhibited excellent sensitivity of upto 1cm. 

#### However accurate or precise, 

##### 1. UWband based localization systems are very expensive 
##### 2. Have high power requirements
##### 3. Need regular maintainence

## Proposed Solution:

### Hardware:
<b> 
1. Raspberry Pi 0 ($5)

2. WiFi routers in the environment (that are mostly already installed in indoor environments)
</b>
Performance of WiFi based localization systems can be improved significantly by using Intelligent Calibration Techniques. Although this method observes a trade off in precision and sensitivity of the sensor but both are well within tolerance for the considered applications.

### Correlation algorithms:
#### Main aim of development of these algorithms was to obtain Distance as a function of RSSI values.
Data of Distance and RSSI values were acquired.
After detailed preprocessing and, training and testing over various degrees of polynomial regression and information entropy based algorithms, the optimized model was chosen.

A new prediction function is made in order to invert the operations done while preprocessing. Now, this function can be directly used to predict Distance based on RSSI values. 

## Observed imporovement in functioning:
#### 1. Speed: needs less than 0.75ms to make predictions.
#### 2. Accuracy: 82.07%
#### 3. Precision: 10cm
