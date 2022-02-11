# intrepid_sim 
RB-Vogui + Kinova Jaco Intrepid simulation repository 

## Install repository

Download repository:

`git clone --recurse-submodules https://github.com/RobotnikAutomation/intrepid_sim` 

Install RB-Vogui controller libraries:

`sudo dpkg -i src/intrepid_sim/rbvogui_common/libraries/*`

Compile repository:

`catkin build`

## Run simulation

To launch simulation:

`roslaunch intrepid_sim_bringup intrepid_complete.launch`

To move the arm: 

`ROS_NAMESPACE=robot rosrun rqt_joint_trajectory_controller rqt_joint_trajectory_controller`

To display available controllers: 

`rosservice call /robot/controller_manager/list_controllers`
