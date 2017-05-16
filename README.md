# CarND - Unscented-Kalman-Filter

[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

This is the project repository for **Project No. 2 Unscented Kalman Filter**, part of Term 2 _Sensor Fusion_ of Udacity Self-Driving Car Nanodegree program, submitted by Albert Killer in May 2017. 

As Unscented Kalman Filter (UKF) was implemented in C++ using the CTRV motion model to process simulated LIDAR and RADAR measurements provided by Udacity. In doing so the position and velocity of an object, moving around a vehicle equiped with those sensors, can be detected with even higher accuracy than achieved by the EKF approach:

```
Accuracy - RMSE:    Accuracy - RMSE:   
px: 0.0972256       px: 0.0972256
py: 0.0853761
vx: 0.4508550
vy: 0.4395880
```
I use a Kalman Filter for LIDAR data. In order to handle the **nonlinear measurement function** _h_(_x_) of RADAR data I apply an Extended Kalmand Filter (EKF). The EKF uses a **linear approximation** of _h_(_x_) and applies _First Order Taylor Expansion_ in order to retrieve a Gaussian distribution again.    

Want to know more about Extended Kalman Filters? Have a look at this one: https://en.wikipedia.org/wiki/Extended_Kalman_filter
