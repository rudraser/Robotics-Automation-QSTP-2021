# Robotics-Automation-QSTP-2021
Automation using ROS
Week I: Unicycle

13.1.2.3 A simple unicycle

![image](https://user-images.githubusercontent.com/83071152/125451990-debd597c-6502-434f-97c3-586ba9bb61b0.png)
 
 Consider the simple model of a unicycle, which is shown in Figure 13.5. Ignoring balancing concerns, there are two action variables. The rider of the unicycle can set the pedaling speed and the orientation of the wheel with respect to the $ z$-axis. Let $ \sigma $ denote the pedaling angular velocity, and let $ r$ be the wheel radius. The speed of the unicycle is $ s = r \sigma$. In this model, the speed is set directly by an action variable $ u_s$ (alternatively, the pedaling rate could be an action variable $ u_\sigma$, and the speed is derived as $ s = r u_\sigma$). Let $ \omega$ be the angular velocity of the unicycle orientation in the $ xy$ plane (hence, $ \omega = {\dot \theta}$). Let $ \omega$ be directly set by an action variable $ u_\omega $. The configuration transition equation is 

 ![image](https://user-images.githubusercontent.com/83071152/125452071-e4b7f7d1-ced1-44bb-ac2c-efd141a03814.png)
 
 This is just the differential drive equation (13.17) with $ L = 1$ and the substitution $ u_s = r u_\sigma$. Thus, a differential drive can simulate a unicycle. This may seem strange; however, it is possible because these models do not consider dynamics. Note that the unicycle can also simulate the simple-car model. Therefore, the tricycle and unicycle models are similar. 
