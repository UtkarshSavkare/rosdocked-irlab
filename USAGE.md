### instructions to run


Modification to the icclab_summit_xl repo 

For performing Autonomus exploration: 

1. In config/global_planner_params.yaml ,Set allow_unknown: true     # Allow planner to plan through unknown space
2. Addition of new move base client python file to suscribe to geometry/msgs, scripts/move_base_client.py
3. Addition of exploration parameters file, config/explore.yaml

For SLAM with Camera:

1. new launch file launch/irlab_summit_xl_gmappingcam.launch for depth image to laser scan for gmapping
2. new launch file launch/slam_gmappingcam.launch with scan topic changed for camera

Modification to the m-explore repo

1. new launch file explore/launch/auto_slam.launch for implementing SLAM autonomously.
```
git clone https://github.com/UtkarshSavkare/icclab_summit_xl.git
git clone https://github.com/UtkarshSavkare/m-explore.git
```
