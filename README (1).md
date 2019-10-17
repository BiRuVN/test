#1 cài đặt
1.Trước tiên cần cài đặt Ubuntu 16.04 hoặc 18.04 ( ros.org hình như chỉ hỗ trợ tới 18.04 )
2.Cài đặt CUDA toolkit và CUDNN cho máy.và cài tensorflow
https://gist.github.com/bogdan-kulynych/f64eb148eeef9696c70d485a76e42c3a
or
https://github.com/hoangtnm/docs/blob/master/Setup-machine-for-Deep_Learning.md
3.cài các gói thư viện
OpenCV. cài từ source or pip
____cài từ source
https://www.facebook.com/cuocduaso/videos/2125267247725141/
____cài từ pip
pip3 install opencv-python
pip3 install opencv-contrib-python
các thư viện khác: cú pháp pip3 install <package>
- scipy
- tensorflow-gpu==1.14.0
- rospkg
- roslib
- rospy 

4.cài ros
Lựa chọn 1 trong 2 phiên bản ROS sau:
Cài đặt ROS Lunar: http://wiki.ros.org/lunar/Installation/Ubuntu
Cài đặt ROS Melodic: http://wiki.ros.org/melodic/Installation/Ubuntu 
ros Melodic là bản ros mới nhất
Chú ý: cần cài đặt bản đầy đủ. Ví dụ với ROS melodic thì cài đặt bản đầy đủ như sau:
sudo apt-get install ros-melodic-desktop-full
Hoàn Thiện đầy đủ các bước từ mục 1.1 đến 1.7
Tạo ROS Workspace
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make
echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc
source ~/.bashrc
Cài đặt rosbridge-suite
sudo apt-get install ros-melodic-rosbridge-server

