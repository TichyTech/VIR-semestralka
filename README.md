# About:

Code for our Team Semestral project in Cybernetics and Robotics course at [Faculty of Electrical Engineering](https://fel.cvut.cz/cs) at [Czech Technical University in Prague](https://www.cvut.cz/en/). 

The goal was to train a neural network policy to control a quadcopter and avoid obstacles using onboard camera sensor. The control policy is a simple 3 layer fully connected neural network with the image from the camera as input and desired velocity at its output. The network is trained via the [Proximal Policy Optimization](https://en.wikipedia.org/wiki/Proximal_policy_optimization) algorithm. The policy is trained and evaluated in our custom environment using the [AirSim](https://microsoft.github.io/AirSim/) Unreal Engine plugin.

The resulting policy performance is used in this video:
<p align="center"><a href="https://www.youtube.com/watch?v=NFOZBlzWg-0&ab_channel=Tom%C3%A1%C5%A1Tich%C3%BD">
<img src="https://img.youtube.com/vi/NFOZBlzWg-0/0.jpg" alt="Video">
</a></p>

### HOW TO: Switch main display rendering off
Open settings.json file from Documents/Airsim and add the following option:
  ```json 
  "ViewMode": "NoDisplay"
  ```
Than you can start AirSim simulation and the screen should be black.

### HOW TO: speed up simulation speed
Open settings.json file from Documents/Airsim and add the following option:
```json
 "ClockSpeed": 1
```
1 is the clock speed multiplier. You should be able to set it to any positive number. A value too large might affect simulation accuracy though.

See [settings](https://microsoft.github.io/AirSim/docs/settings/#viewmode) for more info.
