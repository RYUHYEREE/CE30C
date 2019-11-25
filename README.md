    how to use CE30-C LiDAR on ubuntu18.04, ROS melodic environment.
    
    
    
    
    1. https://github.com/CE30C 에서 SDK-for-linux, SDK-for-ROS를 catkin_ws에 download 하고 압축을 푼다.
    (Download SDK from https://github.com/CE30C and extract SDK-for-linux and SDK-for-ROS to catkin_ws.)
    
    2. SDK-for-linux를 리컴파일한다. 생성된 .so파일을 SDK-for-ROS의 .so파일을 대체하고 make. cm.
        ( (1) Recompile SDK-for-linux. 
          (2) and replace .so file in SDK-for-ROS to the new .so file from SDK-for-linux.
          (3) make and catkin_make )
    
    3. manual 문서를 참고하여 ip설정 변경.
    (change the ip setting.)
    
    
    4. launch 폴더로 이동한 후, source ~/catkin_ws/devel/setup.bash 입력
    (Go to the launch directory and typing source ~ / catkin_ws / devel / setup.bash on terminal.)
    
    5. roslaunch(라이더와의 연결확인)
    
    6. rostopic, rviz 등으로 topic 확인
    (see the topic and signals via rostopic and rviz and so on)
    
    7. src폴더 내 listener.cpp 를 rosrun한다.
    (rosrun listener.cpp)
    
    8. 물체 각도와 거리 데이터 확인 가능.
    (then you can see the object's distance and degree information on new terminal)
