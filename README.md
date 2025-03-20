## Extended Kalman Filter: Range-Only Tracking
This project implements an **Extended Kalman Filter (EKF)** for range-only tracking, a common problem in robotics and autonomous systems. The EKF is used to estimate the state of a moving object (e.g., a robot or vehicle) based on noisy range measurements from a sensor. The implementation demonstrates how to handle non-linear systems by linearizing the process and measurement models at each time step. The project includes:  
- Simulation of a moving object with a known trajectory.  
- Generation of noisy range measurements.  
- Implementation of the EKF algorithm to estimate the object's position and velocity.  
- Visualization of the true trajectory, noisy measurements, and EKF estimates for performance evaluation.  

This project is ideal for those interested in state estimation, sensor fusion, or robotics, and serves as a practical introduction to non-linear filtering techniques.

## Demo Video  
Here’s a demo video showcasing the EKF in action for a simple circular reference trajectory:  

![demo_video GIF](./demo_video.gif)

## Error Plots and 3-Sigma Bounds  
The following plots show the **error covariance** and **3-sigma bounds** for the estimated states over time. These plots help visualize the performance and uncertainty of the EKF.

![Error Covariance Plots](./error_cov_plots_ekf.png)

### Explanation of the Plots:
- **Error Covariance (\(P\))**: The plots show the error covariance for different states (e.g., position, velocity, orientation) over time. The error covariance represents the uncertainty in the EKF's estimates.
- **3-Sigma Bounds**: The shaded regions represent the **3-sigma bounds**, which indicate the confidence interval for the estimates. If the errors stay within these bounds, the filter is performing well.
- **States Tracked**: The states include position (\(P_n\), \(P_d\)), velocity (\(V\)), orientation (\(\psi\)), and other relevant variables. Each plot corresponds to a specific state, showing how the error and uncertainty evolve over time.

## Packages Required  
To run this project, you’ll need the following Python packages:  
- `numpy`  
- `matplotlib`  
- `scipy`  

These packages are commonly used for numerical computations, visualization, and scientific computing.

## How to Run  

### 1. Open in Google Colab  
Click the link below to open the notebook directly in Google Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ladyraga/Non-Linear-State-Estimation-/blob/main/Extended%20Kalman%20Filter_%20range%20only.ipynb)  

### 2. Run Locally  
- Clone this repository:  
  ```bash
  git clone https://github.com/ladyraga/Non-Linear-State-Estimation-.git
