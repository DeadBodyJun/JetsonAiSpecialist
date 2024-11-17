# JetsonAiSpecialist
# Nvidia AI Specialist Certification

<aside>
💡

**OverView of the Project**

프로젝트 개요

- Opening background information (내 프로젝트의 전반적인 문맥을 위해서 필요!)

- General description of the current project (프 로젝트의 전반적인 설명)

- Proposed idea for enhancements to the project (제안하고 싶은 프로젝트의 강점)

- Value and significance of this project (중요성)

- Current limitations (직면하고 있는 한계)

- Literature review(전반적인 프로젝트의 배경지식 공유를 위해서!)

</aside>

# Title

[주제]

DoorSense: 휴머노이드 로봇의 문 인식 시스템

# Opening background information

[ 배경 정보 ]

<aside>
✅ 휴머노이드 로봇이 실내 환경에서 자율적으로 이동하고 작업하기 위해 주변의 장애물과 사물을 인식하고 피할 수 있는 능력이 필요하였음. 이를 위해 문고리와 같은 특정 사물을 인식하는 것이 중요하였고, 문과 같은 구조물을 전체적으로 인지함으로써 로봇이 이동 경로를 효율적으로 설정하고 필요에 따라 회피할 수 있도록 하였음. YOLOv5와 같은 딥러닝 기반 객체 인식 기술은 이러한 기능을 구현하는 데 적합하였고, 특히 실시간으로 문고리와 같은 작은 물체도 정확히 탐지할 수 있어 로봇이 환경을 이해하고 적응하도록 하였음. 본 프로젝트는 YOLOv5를 활용해 문고리를 인식하고, 이를 휴머노이드 로봇의 장애물 인식 시스템에 적용함으로써 스마트홈, 서비스 로봇 등 다양한 분야에서 로봇 활용 가능성을 높이고자 함.

</aside>

- Humanoid robots require the ability to recognize and avoid obstacles and objects in their surroundings to autonomously navigate and operate within indoor environments. For this purpose, recognizing specific objects, such as door handles, is essential, allowing the robot to perceive entire door structures and efficiently plan its routes while avoiding obstacles when necessary. YOLOv5, a deep learning-based object recognition technology, is well-suited to implement these capabilities, enabling the robot to accurately detect small objects like door handles in real-time, thereby enhancing its understanding and adaptation to its environment. This project aims to apply YOLOv5 to recognize door handles and integrate this capability into the humanoid robot's obstacle detection system, thereby increasing the potential for robot utilization in various fields such as smart homes and service robots.
- 

# General description of the current project

[프로젝트 전반적인 설명]

<aside>
✅ 이 프로젝트는 휴머노이드 로봇이 실내 환경에서 자율적으로 문을 인식할 수 있도록 하는 시스템을 개발하는 것을 목표로 한다. 문고리를 다양한 각도와 조건에서 촬영하여 YOLOv5 기반 모델에 학습시키고, 이 학습 모델을 통해 로봇 전방의 특정 거리(`n` 값으로 설정된 범위) 내에서 문고리를 인식하게 한다. 문고리가 감지되면 로봇은 이를 "문이 있다"라고 판단하여, 경로를 회피하거나 문을 여는 동작을 준비하는 등 상황에 맞는 반응을 할 수 있다. 이 프로젝트는 휴머노이드 로봇의 내비게이션 능력을 향상시켜, 스마트홈과 서비스 로봇 분야 등에서 자율 이동성을 높이고 다양한 활용 가능성을 열어줄 수 있다.

</aside>

- This project aims to develop a system that enables humanoid robots to autonomously recognize doors in indoor environments. By capturing images of door handles from various angles and conditions and training a YOLOv5-based model, the robot can recognize door handles within a specific distance (defined as an `n` value) in front of it. When a door handle is detected, the robot interprets this as a "door present," allowing it to respond appropriately by either avoiding the path or preparing to open the door. This project enhances the navigation capabilities of humanoid robots, expanding their potential applications in fields like smart homes and service robotics, ultimately improving autonomous mobility.

### Value and signifiance of the project

[ 프로젝트의 중요성] 

<aside>
💡

이 프로젝트는 실내 자율 로봇의 발전과 사용자 접근성 향상에 중요한 역할을 합니다. 문고리와 같은 작은 물체를 인식함으로써 로봇이 문과 같은 구조물을 탐지하고 회피하거나 상호작용할 수 있어, 스마트홈, 병원, 호텔 등 다양한 실내 환경에서 유연하게 작동할 수 있습니다. 특히, 고도화된 장애물 인식 기술을 통해 복잡한 환경에서도 안정적으로 이동하며, 이를 통해 고령자와 장애인에게도 더 높은 접근성을 제공하여 실용적이고 맞춤형 서비스를 가능하게 합니다. 또한, 이 프로젝트는 자율 로봇이 다양한 실내외 환경에서 사람을 돕고 임무를 수행할 수 있는 기초 기술로 자리 잡아, 향후 로봇의 활용성을 더욱 확대할 잠재력이 있습니다.

</aside>

- This project plays a key role in advancing indoor autonomous robots and enhancing user accessibility. By recognizing small objects like door handles, the robot can detect, avoid, or interact with structures like doors, allowing it to operate flexibly in various indoor environments such as smart homes, hospitals, and hotels. Particularly, this advanced obstacle detection technology enables stable navigation even in complex settings, providing greater accessibility for elderly and disabled users, allowing for practical and personalized services. Furthermore, this project establishes foundational technology for autonomous robots to assist people and perform tasks in diverse environments, offering significant potential for expanded robot applications in the future.

### **Current limitations**

[직면하고 있는 한계]

<aside>
✅ 이 프로젝트는 다양한 한계에 직면하고 있습니다. 먼저, 문고리는 모양, 색상, 위치, 조명 조건에 따라 인식이 어려워질 수 있어 다양한 환경에서 일관된 성능을 유지하기 어렵습니다. 또한, 현재 설정된 거리 내에서만 문고리를 탐지할 수 있어 로봇이 멀리 있는 문고리를 인식하는 데 한계가 있습니다. 실시간 객체 인식에는 높은 계산 자원이 요구되며, 이는 휴머노이드 로봇의 배터리 소모와 비용 증가를 초래할 수 있습니다. 더불어, 문고리를 인식하는 것만으로는 충분하지 않으며 실제로 문을 여는 동작을 수행하려면 추가적인 기계적 설계가 필요합니다. 다양한 형태의 문고리를 인식하기 위해서는 방대한 데이터와 학습 시간이 요구되어 프로젝트 진행에 어려움이 발생할 수 있습니다.

</aside>

- This project faces several limitations. First, recognizing door handles can be challenging due to variations in shape, color, position, and lighting conditions, making it difficult to maintain consistent performance across different environments. Additionally, the system can only detect door handles within a set range, limiting the robot's ability to recognize handles at a distance. Real-time object detection requires high computational resources, which can lead to increased battery consumption and costs for humanoid robots. Furthermore, simply recognizing the door handle is insufficient; additional mechanical design is required for the robot to actually open doors. To recognize various types of door handles, extensive data and training time are required, posing challenges for project progress.

### **Literature review**

[문헌 고찰]

<aside>
💡

1. **로봇의 실내 내비게이션**
    
    실내 환경에서 자율적으로 이동하는 로봇의 내비게이션 기술은 지속적인 연구의 대상이 되고 있습니다. 특히, 로봇이 사람의 도움 없이도 주변 환경을 이해하고 장애물을 회피할 수 있는 능력은 스마트홈, 의료시설, 상업 공간 등에서 로봇의 활용 가능성을 확대하고 있습니다. 최근 연구들은 로봇의 자율 내비게이션을 위해 SLAM(Simultaneous Localization and Mapping), 레이저 센서, 초음파 센서, 카메라 비전을 결합한 다양한 접근 방식을 활용하고 있으며, 특히 카메라 비전 기반의 내비게이션 시스템이 실내 로봇 내비게이션에서 중요한 요소로 자리 잡고 있습니다.
    
2. **객체 인식 기술**
    
    객체 인식 기술은 로봇이 특정 물체를 식별하고 인식하는 데 핵심적인 역할을 합니다. 특히 YOLO(You Only Look Once)와 같은 실시간 객체 탐지 모델은 신속하고 정확한 객체 인식을 위해 많이 사용되고 있습니다. YOLOv5는 이전 버전보다 성능과 속도가 향상된 모델로, 다양한 객체 인식 연구에서 실시간 인식이 필요한 응용 분야에 적합한 성능을 보이고 있습니다. 연구에 따르면, YOLOv5는 작은 물체의 인식 정확도가 높아 로봇이 실내에서 문고리와 같은 특정 물체를 식별하는 데 효과적입니다.
    
3. **장애물 탐지와 자율 이동**
    
    자율 이동 로봇의 개발에서 장애물 탐지는 매우 중요한 역할을 합니다. 이를 위해 많은 연구들이 센서 기반 탐지 기술과 딥러닝 기반 인식 기술을 결합하고 있습니다. 일반적인 센서 탐지와는 달리, 딥러닝 기반 탐지 기술은 로봇이 주변 환경을 더 정교하게 인식하고, 예측 가능한 경로를 계획하는 데 유용합니다. 문고리와 같은 작은 물체를 포함한 장애물 탐지 시스템은 특히 실내 환경에서 장애물 인식의 한계를 극복하고, 로봇의 이동성을 높이기 위한 중요한 연구 과제로 다뤄지고 있습니다.
    
4. **미래의 응용 가능성**
    
    이러한 객체 인식 및 내비게이션 기술의 발전은 휴머노이드 로봇의 활용을 위한 중요한 기반이 됩니다. 현재 스마트홈, 의료 시설, 서비스 산업에서 로봇 활용의 필요성이 증가하고 있으며, 자율 이동 능력을 가진 로봇은 이러한 요구를 충족하는 중요한 역할을 할 수 있습니다. 문고리 인식 프로젝트는 이러한 연구 흐름의 일환으로, 실내 환경에서 로봇이 독립적으로 물체를 인식하고 상호작용할 수 있는 능력을 높이는 것을 목표로 하여 자율 로봇의 실용성을 확장할 수 있는 가능성을 제시합니다.
    
</aside>

1. **Indoor Robot Navigation**
    
    Navigation technology for robots in indoor environments is a constant focus of research, especially as the ability of robots to understand surroundings and avoid obstacles independently increases their potential for use in smart homes, healthcare facilities, and commercial spaces. Recent studies incorporate various approaches, such as combining SLAM (Simultaneous Localization and Mapping), laser sensors, ultrasonic sensors, and camera vision for autonomous robot navigation, with camera vision-based navigation becoming a key component for indoor robot navigation.
    
2. **Object Recognition Technology**
    
    Object recognition plays a crucial role in enabling robots to identify specific objects. Models like YOLO (You Only Look Once) are widely used for fast, accurate object detection, with YOLOv5 offering enhanced performance and speed compared to previous versions. Research shows that YOLOv5 is particularly effective for real-time recognition, especially for small objects, making it suitable for identifying specific items like door handles in indoor environments.
    
3. **Obstacle Detection and Autonomous Movement**
    
    Obstacle detection is critical in developing autonomous robots. Numerous studies combine sensor-based detection and deep learning-based recognition technology, with deep learning helping robots more precisely interpret their surroundings and plan routes predictively. Obstacle detection systems capable of recognizing small objects like door handles are essential for overcoming limitations in indoor obstacle recognition and improving robot mobility.
    
4. **Future Applications**
    
    Advances in object recognition and navigation technology provide a solid foundation for the application of humanoid robots. The need for robots in smart homes, healthcare, and service industries is growing, and autonomous robots with navigation capabilities are poised to meet these demands. This project aligns with this research trend, aiming to improve robots' ability to independently recognize and interact with objects in indoor settings, suggesting greater utility for autonomous robots.
    

## **영상 취득 방법 (Image Acquisition Method):**

- 실제 실내의 문고리를 다각도로 촬영 하였다
Captured actual indoor door handles from various angles.

(https://youtube.com/shorts/IZqbfBX37iw?feature=share)

## 학습 데이터 추출과 학습 어노테이션 (**Learning Data Extraction and Learning Annotation)**:

YOLOv5에서 640 해상도 이미지로 학습하기 위해서 먼저 영상을 640 x 640 해상도 영상으로 만들었다.  

To learn from YOLOv5 with 640 resolution images, we first made the images into 640 x 640 resolution images.

### 비디오 해상 조정 (Video resolution adjustment)

![image.png](image.png)

640 x 640 해상도로 만들어진 영상을 프레임 단위로 이미지로 만들거나 어노테이션을 하기 위해서 Video/Image Labeling and Annotation Tool로 잘 알려진 DarkLabel을 사용했다.

DarkLabel, also known as Video/Image Labeling and Annotation Tool, was used to image or annotate images made at 640 x 640 resolution in frame units.

![image.png](image%201.png)

DarkLabel 프로그램에서 영상을 프레임 단위로 이미지로 변환할 수 있다. 먼저 Open Video를 통해 640 x 640 해상도 영상을 선택한다. 이후 labeled frames only가 체크 표시가 활성화 되어 있을텐데 체크 표시를 비활성화한다. 이후 as images를 통해 images라는 폴더 안에 이미지로 변환한다.

In the DarkLabel program, an image can be converted into an image in units of frames. First, a 640 x 640 resolution image is selected through Open Video. After that, labeled frames only will have the check mark enabled but deactivate the check mark. After that, it is converted into an image in a folder called images through as images


학습에 필요한 라이브러리
```
import torch
import os
from IPython.display import Image, clear_output  # to display images
```

학습 스크립트
```
python "C:\\Users\\ASUS\\Desktop\\AI\\yolov5\\yolov5\\train.py"  --img 512 --batch 16 --epochs 300 --data C:\Users\ASUS\Desktop\AI\yolov5\yolov5\data.yaml --weights yolov5n.pt --cache
```

<img width="858" alt="KakaoTalk_20241117_222321158" src="https://github.com/user-attachments/assets/f8bf26cc-afc7-4d91-ba4f-8d2bb23b8d6b">

cmd 환경에서 학습을 돌리는 모습



```img 512```: 입력 이미지의 크기를 512*512로 설정한다.
Set the size of the input image to 640x640.

```batch 16```: 배치 크기를 설정한다. 한 번에 처리되는 이미지의 수를 나타낸다.
Sets the batch size. This indicates the number of images to be processed at one time.

```epochs 300```: 학습할 총 에폭(epoch) 수를 설정합니다.
Sets the total number of epochs to learn.

```C:\Users\ASUS\Desktop\AI\yolov5\yolov5\data.yaml```: 데이터셋 및 모델 구성에 대한 설정이 담긴 YAML 파일의 경로를 지정한다.
Specifies the path to the YAML file containing the configuration settings for the YOLOv5 model.

```weights yolov5n.pt```: 미리 훈련된 가중치 파일의 경로를 지정한다. 여기서는 yolov5n.pt 파일을 사용하고 있다.
Specifies the path to the pre-trained weights file. Here, we are using the yolov5n.pt file.


Nvidia Jetson Nano 학습 결과 Nvidia Jetson Nano Training Result
학습 결과는 ```C:\Users\ASUS\Desktop\AI\yolov5\yolov5\runs/train```에 저장된다.
Training results are stored in ```C:\Users\ASUS\Desktop\AI\yolov5\yolov5\runs/train```

![F1_curve](https://github.com/user-attachments/assets/27ee4581-89eb-434f-a4ea-1f97f3b77978)
![PR_curve](https://github.com/user-attachments/assets/278371ed-1620-4129-8320-96e38b511e37)
![P_curve](https://github.com/user-attachments/assets/3411faf9-003c-48cb-acb1-2f961d5abfea)
![R_curve](https://github.com/user-attachments/assets/ac18c2af-10b3-4355-9f66-dc6b10341832)

![results](https://github.com/user-attachments/assets/c21f2240-7f10-40c4-8152-3a18985fc0b8)


Nvidia Jetson Nano 학습 결과 검증 영상 Nvidia Jetson Nano Training Results Verification Video

카메라를 뒤집어도 정확하게 문고리를 감지해낸다

JetsonAiSpecialist verification1
https://youtube.com/shorts/6gejM1pBcUc?feature=share

JetsonAiSpecialist verification2
https://youtube.com/shorts/sqgctFothtA?feature=share



