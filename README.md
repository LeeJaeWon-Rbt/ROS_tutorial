# ROS_tutorial


## Ubuntu와 ROS 기본학습
- Ubuntu 14.04와 ROS indigo 설치 및 개발환경 설정
- 추후 실제 개발과 다른 버전의 ROS 사용을 위한 기본 학습  
- Oracle VM VirtualBox 사용  

## Ubuntu 16.04 + ROS Kinetic
- https://releases.ubuntu.com/xenial/
- http://wiki.ros.org/kinetic/Installation/Ubuntu
- ROS Kinetic ONLY supports Wily (Ubuntu 15.10), Xenial (Ubuntu 16.04) and Jessie (Debian 8) for debian packages.  

- ### Part 1
  1. Ubuntu 16.04(LTS) 설치
  2. `sudo apt-get install chrony`  
  3. `sudo apt-get install ntpdate`  
  4. `sudo ntpdate ntp.ubuntu.com` -> 서버시간 동기화  
  5. http://wiki.ros.org/kinetic/Installation/Ubuntu의 1.4 Installation의 첫번째까지 진행 후  
  6. `sudo apt-get upgrade` 진행  

- ### Part 2
  1. http://wiki.ros.org/kinetic/Installation/Ubuntu
  2. `sudo apt-get install ros-kinetic-desktop-full`
  3. `sudo apt-get install python-rosinstall`  
  4. `sudo apt-get install ros-kinetic-rqt-*`  
  5. `sudo rosdep init` -> 초기화
  6. `rosdep update` 

- ### Part 3
  1. `gedit ~/.bashrc` 입력 (1.5 Environment setup)  
  -> echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc  
  2. `source /opt/ros/kinetic/setup.bash` 마지막에 설정 추가
  3. 이외의 설정들 (출처: ROBOTIS OpenSourceTeam ROS강의 Chapter3)
  <p align="center"><img src="https://user-images.githubusercontent.com/72693388/108215795-0f7e9b80-7175-11eb-886e-74784c013b50.png" width="500px"></p>  
<p align="center"> 환경 설정 </p>  
  4. 새 터미널을 열고 roscore 실행 여부 확인  
  5. 
 
