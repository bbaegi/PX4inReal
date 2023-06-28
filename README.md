# PX4inReal
PX4 FC 실기체 제작 간 팁들 기록

## Companion PC 세팅

### NVidia Jetson Orin Nano
* Install Jetpack - (23.06.28 5.10.104-tegra)
```bash
sudo apt update
sudo apt upgrade
```

* Install ROS noetic
ROS Noetic Official Install Guide Link : <http://wiki.ros.org/noetic/Installation>
* Install MAVROS (ROS noetic)
```bash
sudo apt-get install ros-noetic-mavros ros-noetic-mavros-extras ros-noetic-mavros-msgs
```
* Install GeographicLib
```bash
wget https://raw.githubusercontent.com/mavlink/mavros/master/mavros/scripts/install_geographiclib_datasets.sh
sudo bash ./install_geographiclib_datasets.sh   
```

### NVidia Jetson Nano
*install MAVROS  
*install GeographicLib  
*fcu_url="/dev/ttyTHS1"

## PX4 세팅

### Serial 통신 포트 설정
* 기본적으로 PX4는 주로 Radio Telemetry를 장착해서 사용하는 telem1 포트만 MavLink가 활성화 되어있다.
