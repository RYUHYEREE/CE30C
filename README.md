1.	https://github.com/CE30C 에서 SDK-for-linux, SDK-for-ROS를 workspace에 download 하고 압축을 푼다.
2.	SDK-for-linux를 리컴파일한다. 생성된 .so파일로 SDK-for-ROS의 .so파일을 대체하고 make. cm.
3.	manual 문서를 참고하여 ip설정을 변경한다.
1)	xavier 네트워크 설정 ipv4설정을 ip adress 192.168.1.2, subnet mask를 255.255.255.0,
gateway는 비운다.
2)	ping을 통해 확인한다.

4.	launch 폴더로 이동한 후, source ~/catkin_ws/devel/setup.bash 입력(설정에 따라 상이)
5.	roslaunch(라이더와의 연결확인)
6.	rostopic, rviz 등으로 topic 확인
7.	src폴더 내 listener.cpp 를 rosrun한다.
8.	물체 각도와 거리 데이터 확인 가능.
