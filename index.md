# Welcome to Ryan's Pages!

This is the personal GitHub page of Zirui (Ryan) Zhao.<br/>

  **Zirui Zhao**<br/> 
  Bachelor of Engineering in Automation (EECS) , will graduate in 2020 <br/>
  Department of Automation Science and Engineering <br/>
  The School of Electronic and Information Engineering<br/>
  Xi'an Jiaotong University<br/>
  No.28 Xianning West Road, Xi'an 710049, P.R.China.<br/>
  Email: ryan_zzr@outlook.com<br/>
  Welcome to my [GitHub profile](https://github.com/1989Ryan).<br/>
  Download my [CV](https://github.com/1989Ryan/README_pictures/raw/master/images/Zirui_Zhao_CV.pdf).<br/>
  
## Research interests

  I am interested in the Robotics and its combination with machine learning. In particular, I am very interested in the Robotic Cognition, Multi-Robot System, Robotic Reasoning. <br/>
  I am currently focusing on the semantic SLAM and how to let robot navigate like human with semantic infomation. <br/>

## Current Applied Research Project
**Multi-agent Collaborative Navigation in robots, Exploration and Structured Semantic Information Establishment IAIR XJTU (April. 2018 – now)**<br/>

  I joined in the lab of Institute of Artificial Intelligence and Robotics (IAIR) and I’m currently working on the research of multi-agent collaborative navigation, which aims to actualize the coordinate navigation and exploration task using DJI UAV and autonomous vehicle. Meanwhile, this project is trying to use the semantic information for visual navigation, human-robot interaction and data fusion to build a joint semantic-metric inference framework. This project is a long period project and a group work since robotic system development is a complicated work. And I am the group leader under the faculty superviso, Dr. Pengju Ren.
  
  Our robot consists of UAV and UGV.

<center><img src="https://raw.githubusercontent.com/1989Ryan/README_pictures/master/images/46701763-26CE-477C-82B4-D00BF45289B0.jpeg" height="75%" width="75%"/>  
 <p align="center">DJI UAV</p>
 
 <img src="https://raw.githubusercontent.com/1989Ryan/README_pictures/master/images/08743A5F-3D03-4511-870B-D1B1A6E6DAE4.png" height="75%" width="75%"/>
<p align="center">MIT Racebot</p>

<img src="https://raw.githubusercontent.com/1989Ryan/README_pictures/master/images/B660E119-F653-4B3D-97EF-8D490B7C1EC0.jpeg" height="75%" width="75%"/></center>
<p align="center">YOUIBOT</p>

### Motivation

We were inspired by homan perception system. How can we human-beings manage to navigate with visual imformation. Human will never build a precise 3D map to navigate from one place to the other. The only sensor we use is our eyes. Visual information contains all the necessary information we need. So how to let a robot grap the various information including the distances and semantic meaning, and use them for self-navigation, is the premary problem that I want to solve. 

Also, the UAVs and UGVs, in some aspects, are complementary to each other, since the UAVs can catch the global situation and UGVs are more convenient for human-robot interaction. Their combination will greatly enhance their ability.

### Completed Tasks, Implementations and Methodologies
  
  We try to in-complement the autonomous driving of small robotic vehicle and the cooperation of UAV and robotic vehicle. The UAV is responsible for the path planning of the vehicle and helps the automatic follow-up of the vehicle with computer vision technology. In this project, my job is mainly on the inference acceleration of neural network and the movement control of the UAV and robotic vehicle using ROS and CV. I’m currently studying the self-navigating of ground vehicle with a given map. We try to utilized the pictures captured by UAV to build a map automatically and send it to the ground vehicle robots for self-navigation. And these work includes the technology of path planning, obstacle avoidance, transformation of coordinates and communication between multi-agents.
  
There are some implementations of SLAM and detection algorithm.

<center><img src="https://github.com/1989Ryan/README_pictures/blob/master/images/952E7C77-474F-45BE-8EA2-E8107784FFDE.gif?raw=true" height="75%" width="75%"/></center>

<p align="center">Laser Slam</p>

<center><img src="https://github.com/1989Ryan/README_pictures/blob/master/images/FB4F695E-3721-4285-ACFA-177B0819FFA2.gif?raw=true"/></center>

<p align="center">Visual Slam</p>

<center><img src="https://github.com/1989Ryan/README_pictures/blob/master/images/ED65AE93-CDAD-45A3-BFCC-AE02F78EC1C7.gif?raw=true" height="75%" width="75%"/></center>

<p align="center">Detection and tracking in UAV</p>

  Our baseline model is try to implement the laser-scan as the main sensor for cognition and navigation. The UAV will flying in the air and establish the global cost map for UGV. The global cost map is built by image segmentation. The UGV will go through a small labyrinth. We try to utilize the TEB algorithm for global path-planning and it shows great robustness during our experiment.
  
<center><img src="https://github.com/1989Ryan/README_pictures/blob/master/images/2019-01-21%20172348.png?raw=true" /></center>
<p align="center">Project Design</p>

### Demo
  
  You can watch our demo video about multi-agent system going through a labyrinth.
  
  <center><iframe width="560" height="315" src="https://www.youtube.com/embed/wSB4hyW9rWc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>
  
### Current Problems
  
  However, the stability and power consuming is not desirable for on-board system. Therefore, we try to move on to the visual information for cognition, navigation and path-planning. We try to implement Monocular ORB-SLAM, which is a robust, state-of-the-art and open-source visual SLAM algorithm, for re-localization and navigation. We also try to use high-resolution image for road segmentation and cost map building. We have proved that the ORB-SLAM is suitable for urban area re-localization and mapping. And our problem is cooperation and planning through visual information, including dynamic regional path-planning and multi-agent communication.

## Previous Research & Contest Experiences
**1.	Machine learning & Computer Vision Open Experiment Program IAIR XJTU (Sept. 2017 – April. 2018)**<br/>
  Computer vision is currently changing the world with marvelous accuracy of image classification, target detection and pattern recognition. I learned the basic knowledge of computer vision as well as the framework of TensorFlow from my advisor of an open experimental program, which is set specifically for those undergraduates that are willing to participate in basic study of convolutional neural network and computer vision, from Institute of Artificial Intelligence and Robotics, XJTU. During this period, I read the book “Deep Learning” written by Goodfellow, which contains a large number of knowledges of mathematics and statistics that I was currently studying. After that, I used TensorFlow to actualize the first computer vision program based on the dataset called MNIST. Then I tried to use ResNet50 to finish the image classification task based on the dataset CIFAR-100. Besides, I also participated in a contest about computer vision held by Baidu and XJTU in 2018 using SE-ResNet152 to solve 100-brand classification problems and got national rank 39 / 300. Besides, I also particpated in the DAC system design contest and finally got rank 4/21.
<center><img src="https://raw.githubusercontent.com/1989Ryan/README_pictures/master/images/730C6A64-4992-454F-ADCA-82B720EC3237.jpeg"/></center>

**2.  Tele-Robotic and Deep Learning Project NUS SoC Summer Workshop 2018 (July. 2018 - August. 2018)**<br/>
  Computer vision is unprecedentedly popular, and I believe that computer vision will be widely applied in autonomous robot for specific task such as rescuing after disaster or exploring unknown area. When I was participating in the NUS SoC Summer Workshop 2018, I chose the project called “Tele-Robotics and Deep learning” which was the first autonomous robot and robotic vision project that I had participated in. Then I learned the basic knowledge of the embedded system and control theory of robotic movement, and how to use computer vision algorithm in robotics. We used the Raspberry Pi and Arduino Mega 2560 to build a simple blind-guide robotic vehicle with ultrasonic sensors, IMU and Pi camera. We used the cloud service of Azure to accelerate the inference of Inception-v3 neural network which is responsible for the computer vision task to recognize the obstacles. Obstacle avoidance is utilized in this project which is enforced by using different sensors to detect obstacles and control the movement. In this project, I was the leader of our team, helping to negotiate with other teammates and responsible for designing the overall frame of the robotics, including the embedded system and computer vision algorithm. And I was the monitor of the lab who was responsible for the students affairs and daily management of lab.
  
<center><img src="https://github.com/1989Ryan/README_pictures/blob/master/33428DCD-E755-40FD-98A3-71FAC864B080.gif?raw=true" height="75%" width="75%" /></center>
<p align="center">demo of our robot, using ultrasonic sensor</p>
<center><img src="https://github.com/1989Ryan/README_pictures/blob/master/images/webwxgetmsgimg.jpg?raw=true" height="75%" width="75%" /></center>
<p align="center">Our team</p>



**3.	2018 Global College Technical Summer Training Camp JD AI Research (August. 2018)**<br/>
 As for the theory of machine learning, I studied the theory of deep neural network not only about the utility of CNN in computer vision, but also about some aspects of pure theory of machine learning. In summer of 2018, I got an opportunity of participating in 2018 Global College Technical Summer Training Camp. And there are only 40 students selected, and I was one of only 2 undergraduates among them. The summer camp is designed to help campers fully understand the frontier issues of AI industry, so as to identify and discover potential excellent future researchers in AI field. In this experience I acquired the theory of adversarial attack of deep neural network which enhanced my knowledge of convolutional neural network. I learned the elementary and advanced methods of adversarial attack such as FGSM, ZOO and One-Pixel attack method as well as the vulnerability of neural network. This experience enhanced my theoretical foundation of convolutional neural network and computer vision. Moreover, I know about the frontier issue of AI industry which cannot be easily acquired in the classroom or lab in university. 

<center><img src="https://raw.githubusercontent.com/1989Ryan/README_pictures/master/images/2535A18E-0B3C-4B96-AEF8-5A104E2BDDA2.jpeg" height="70%" width="70%"/><br/><img src="https://raw.githubusercontent.com/1989Ryan/README_pictures/master/images/1EED6A49-88B3-4D18-BC59-C4144C1CA7D4.jpeg" height="70%" width="70%"/></center>
