# Calib_3LRFs-V1.0
Extrinsic calibration of three LRFs

A refined method from our paper (calibration of IMU and another refined method are coming, perhaps after three months):
```
@article{Yin, D.; Liu, J.; Wu, T.; Liu, K.; Hyyppä, J.; Chen, R. Extrinsic Calibration of 2D Laser Rangefinders Using an Existing Cuboid-Shaped Corridor as the Reference. Sensors 2018, 18, 4371.
}
```

Our paper uses LM algorithm to solve the nonliniear problem, but sometimes it is not stable.
Now we use simplex with multi tries in the method to get more stable result.

# Usage
1. run Calib_3LRF_PreProc.m to preprocess data
2. run Calib_3LRFs.m to do the calibration
3. run Calib_3LRFs_ShowCalibrationResult.m to visualize the calibration result

# Note
We also have codes for generating sythetic data as shown in the paper.
Perhaps you need to make sure the distance unit in the raw data. In currenet version we use meter.