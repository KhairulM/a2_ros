# a2_ros

ROS2 (Jazzy) simulation of the Unitree A2 quadruped using MuJoCo and a trained RL locomotion policy.

## Setup

```bash
conda deactivate   # repeat until $CONDA_PREFIX is empty
git clone git@github.com:ETHZ-RobotX/a2_ros.git --recursive
bash a2_ros/install.sh
```

## Run

Source in every new terminal:
```bash
source a2_ros/setup.sh
```

Launch the simulation:
```bash
ros2 launch a2_ros sim.launch.py
ros2 launch a2_ros sim.launch.py rviz:=true
ros2 launch a2_ros sim.launch.py scene:=scene_terrain.xml
```

## Gamepad

| Input | Action |
|---|---|
| Left stick | Forward / strafe |
| Right stick horizontal | Yaw |
| X + L2 | Sit |
| Triangle + L2 | Stand |
| L2 + R2 | Walk |
