# AI-Task
 *install VirtualBox from https://www.virtualbox.org/

# install Ubuntu 22.04 from https://ubuntu.com/blog/tag/22-04-lts

# install ubuntu in VirtualBox 

# run the commands in ubuntu terminal and follow the instructions {
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

sudo apt-get update

sudo apt-get install ros-kinetic-desktop-full

apt-cache search ros-kinetic

echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc

sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

sudo apt install python-rosdep

sudo rosdep init

rosdep update

sudo apt-get install ros-noetic-catkin

mkdir -p ~/catkin_am/src

cd ~/catkin_am/

catkin_make

cd ~/catkin_am/src

git clone https://github.com/smart-methods/arduino_robot_arm.git 

cd ~/catkin_am

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-kinetic-moveit

sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line
(source /home/amal/catkin_am/devel/setup.bash)
then 
ctrl + o

source ~/.bashrc

roslaunch robot_arm_pkg check_motors.launch }
