# MP_DR_T14
The GitHub repository for DRDO's UAV-Guided UGV Navigation Challenge of Inter-IIT Tech Meet 10.0. Our complete approach and solution is explained [here](https://drive.google.com/file/d/1BoLnpm_vrVwxSM5Zx2mncTXqMaLPVXrA/view?usp=sharing).


## Installation Instructions

- Clone this repository in the `src` folder of your catkin workspace.
- Inside your workspace folder, run `catkin build`.
- Download this [file](https://drive.google.com/file/d/1KeiyFDvNub4L3TZ1F-H8IdRdSsqZHE00/view?usp=sharing) and place it in `catkin_ws/src/MP_DR_T14/interiit22/scripts/`
- To install dependencies
  ```
  rosdep install --from-paths src --ignore-src -r -y
  ```
- To run Gazebo simulation
  - For world 1
    ```
    roslaunch interiit22 drdo_world1.launch
    ```
  - For world 2
    ```
    roslaunch interiit22 drdo_world2.launch
    ```
  - For world 3
    ```
    roslaunch interiit22 drdo_world3.launch
    ```
- To run Ardupilot, in another terminal
  ```
  sim_vehicle.py -v ArduCopter -f gazebo-iris --console
  ```
