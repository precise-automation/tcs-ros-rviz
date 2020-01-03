# pa_rviz_pf3400
A package for visualizing a PF3400 in real time using RViz. Requires TCS to be running on the PF3400.

### Install
*Requires ROS and RViz.*

If you already have a catkin workspace, skip to step 2.
1. Create catkin workspace
   - `cd ~`
   - `mkdir my_workspace`
   - `cd my_workspace`
   - `catkin_make`
2. Navigate to src: `cd src` 
3. Clone project: `git clone .....`
4. Make
   - `cd ~/my_workspace`
   - `catkin_make`

### Run
1. Setup TCS on the controller
2. `source ./devel/setup.bash`
3. `roslaunch pa_viz_pf3400 bridge.launch ip:="192.168.0.1"`

RViz should pop open with a PF3400 loaded and already live updating. If you want
to visualize a GPL project, make sure to load both TCS **and** the other project
using GDE. TCS **must** be running for the visualization to work.


*Permission is granted to customers of Precise Automation to use this software for any purpose, including commercial applications, and to alter it and redistribute it freely, so long as this notice is included with any modified or unmodified version of this software.*

*This software is provided "as is," without warranty of any kind, express or implied.  In no event shall Precise Automation be held liable for any direct, indirect, incidental, special or consequential damages arising out of the use of or inability to use this software.*
