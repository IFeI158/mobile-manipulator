# Mobile Manipulator Robot (지능형 도우미 로봇)

ROS 기반 **모바일 매니퓰레이터(Mobile Manipulator)** 시스템을 구현한 프로젝트입니다.  
사용자가 지정한 물체를 인식하고 해당 위치까지 자율적으로 이동한 뒤 물체를 집어 지정된 위치로 전달하는 **지능형 도우미 로봇**을 개발했습니다.

모바일 매니퓰레이터는 **이동 로봇(Mobile Platform)** 과 **로봇팔(Manipulator)** 을 결합한 시스템으로, 이동성과 물체 조작 능력을 동시에 수행할 수 있습니다.

---

## Project Overview

- **기간** : 2025.03 – 2025.06 (1학기)  
- **인원** : 5명  
- **역할** : Hardware 설계 / Vision 개발  

본 프로젝트에서는 모바일 로봇 플랫폼과 로봇팔을 **직접 설계 및 제작**하고 ROS 기반 제어 시스템을 구축하여 물체 인식 및 자율 이동 기반의 물체 전달 시스템을 구현했습니다.

---

## System Architecture

```
User Input (Mouse)
      ↓
Camera Vision
      ↓
Object Position Calculation
      ↓
Coordinate Transform
      ↓
ROS Navigation
      ↓
Mobile Robot Movement
      ↓
Robot Arm Manipulation
      ↓
Object Pick & Return
```

---

## Key Features

### 1. Object Selection
사용자가 카메라 화면에서 마우스로 물체를 선택하여 목표 물체를 지정

### 2. Vision-based Object Position Estimation
카메라 영상에서 선택된 물체의 좌표를 계산하여 로봇 좌표계로 변환

### 3. Autonomous Navigation
ROS Navigation을 활용하여 목표 위치까지 자율 주행

### 4. Robot Arm Manipulation
로봇팔을 이용한 물체 Pick & Place 동작 수행

### 5. Automatic Return
물체를 집은 후 초기 위치로 복귀

---

## Hardware Design

- Mobile Robot Platform  
- Robot Arm (Manipulator)  
- Camera  
- Lidar Sensor  
- OpenCR Controller  

로봇 하드웨어는 직접 설계 및 제작하여 시스템에 통합하였습니다.

---

## Software Stack

- ROS / ROS2  
- Python  
- OpenCV  
- Gazebo Simulation  
- TurtleBot3  
- Navigation Stack  

---

## Repository Structure

```
mobile-manipulator
│
├── turtlebot3_ws
│   └── src
│
├── ydlidar_ros2_ws
│   └── src
│
├── robotarm_capstone.xacro
│
└── README.md
```

---

## Demonstration

프로젝트 실행 영상 또는 GIF 추가 예정

---

## Future Improvements

- Object Detection 기반 자동 물체 인식  
- MoveIt 기반 로봇팔 Motion Planning  
- Human-Robot Interaction 기능 추가  
- SLAM 기반 환경 인식 개선  

---

## Author

**IFeI158**  
Mechanical Engineering  
Robotics / Autonomous Systems
