# ur_pilz_demo
Demonstration of Pilz Industrial Motion Planner in MoveIt with Universal Robots


<p align="center">
    <img src="docs/demo.gif" alt="gif showing demo of ur_pilz_demo" />
    </br>
    <sup>Sample video showing demonstration on RViz</sup>
</p>


## Dependencies
* **ros-humble-moveit**: Install using the following command: 
    ```console
    $ sudo apt-get install ros-humble-moveit
    ```
* **ros-humble-ur-robot-driver**: Install using the following command: 
    ```console
    $ sudo apt-get install ros-humble-ur-robot-driver
    ```
* **ros-humble-ur-moveit-config**: Install using the following command: 
    ```console
    $ sudo apt-get install ros-humble-ur-moveit-config
    ```


## Compilation
1. Make sure to download complete repository. Use `git clone` or download zip as per convenience.
2. Invoke `colcon` tool inside ros workspace i.e., `colcon build`


## Steps to run
1. Start UR ROS 2 driver in simulation mode by using the following command:
    ```console
    $ ros2 launch ur_robot_driver ur3e.launch.py robot_ip:=yyy.yyy.yyy.yyy \
      use_fake_hardware:=true launch_rviz:=false \
      initial_joint_controller:=scaled_joint_trajectory_controller
    ```
2. Invoke the demo by using the following command:
    ```console
    $ ros2 launch ur_pilz_demo ur_pilz.launch.py 
    ```


## Note
This package has been tested on the following environment configuration-

| Name                        | Value                                  |
| --------------------------- | -------------------------------------- |
| ROS                         | Humble                                 |
| ros-humble-ur-moveit        | 2.5.5-1                                |
| ros-humble-ur-robot-driver  | 2.2.9-1                                |
| ros-humble-ur-moveit-config | 2.2.9-1                                |
| OS                          | Ubuntu 22.04.3 LTS (64-bit)            |
| Kernel                      | Version 6.2.0-35-generic               |
| GCC                         | Version 11.4.0                         |
| Python                      | Version 3.10.12                        |
| RAM                         | 8 GB                                   |
| Processor                   | Intel® Core™ i7-7700 CPU @ 3.60GHz × 8 |


## Issues (or Error Reporting) 
Please check [here](https://github.com/ravijo/ur_pilz_demo/issues) and create issues accordingly.

