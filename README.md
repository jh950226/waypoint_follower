/home/pinky/pinky_violet/src/pinky_violet/pinky_navigation/src/waypoint_follower.py

/home/pinky/pinky_violet/src/pinky_violet/pinky_navigation/CMakeLists.txt

1.위와 비슷한 경로로 파일들이 위치해야함.

2.pinky_violet 폴더에서 colcon build

3.재지환경불러오기(setup.bash)->pinky환경불러오기(local_setup.bash) - 로봇에서

4.터미널 4개 팝업

5.핑키 브링업 노드 실행 (로봇)
실행한 명령어
ros2 launch pinky_bringup bringup.launch.xml

6.핑키 내비게이션 노드 실행(로봇)

맵이 형성이 되어있어야함. 집에서 맵을 만들어서 그 파일로 내비게이션 노드를 실행했음.

실행한 명령어
ros2 launch pinky_navigation bringup_launch.xml map:=my_map.yaml

7.핑키 rviz실행 (local PC)
ros2 launch pinky_navigation nav2_view.launch.xml

8.ros2 run pinky_navigation waypoint_follower 명령어 실행 (로봇)

