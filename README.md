# Robotics2_JacobianandPT_Group1Cartesian_2024-
![Jacobian Matrix](https://github.com/billyabante/Robotics2_JacobianandPT_Group15_Cartesian_2024/assets/157568463/008b7661-9495-4b8e-936f-a6b0986956fc)
![Jacobian Matrix (1)](https://github.com/billyabante/Robotics2_JacobianandPT_Group15_Cartesian_2024/assets/157568463/68a3f066-7b0d-44f3-80d4-47a9ecc97e5b)


# I. Abstract of the Project

This project explores the concepts and steps in controlling the movements of Cartesian Manipulator.A Cartesian manipulator is a type of robot with linear movements along the X, Y, and Z axes, similar to a 3D printer or a CNC machine. To control this robot's movements, we use several mathematical tools and concepts.First,start by calculating the Jacobian Matrix of the Cartesian Manipulator and make also a GUI.The Jacobian Matrix helps us understand how small changes in the robot's joint positions affect the position and orientation of its end-effector (the tool or hand at the end of the robot). By using this matrix, we can calculate velocities and ensure smooth movements.Then compute the singularity,using the determinants of jacobian and basket method.Next,derive the differential equation,it describe the relationship between the robot's joint movements and time. These equations are essential for understanding how the robot's position changes over time and are used to control its speed and acceleration.Lastly,make a path and trajectory planning for timing of movements along that path to ensure efficiency and avoid obstacles.In summary, a Cartesian manipulator uses the Jacobian matrix, differential equations, and path and trajectory planning to move precisely and safely, and to ensure smooth and reliable operations.


# II. Introduction

A Cartesian manipulator, also referred to as a gantry robot or linear robot, is an industrial robot characterized by its movement in straight lines along the Cartesian coordinate system's X, Y, and Z axes. This configuration ensures highly precise and predictable movements, making Cartesian manipulators ideal for tasks that demand high accuracy, such as 3D printing, CNC machining, and automated assembly lines. Unlike articulated robots, which rely on rotating joints, Cartesian manipulators use linear actuators. This use of linear actuators not only simplifies their control and programming but also enhances their reliability and ease of maintenance. Their straightforward design is particularly advantageous for repetitive tasks and contributes to their robustness in industrial settings.

Typically, Cartesian manipulators consist of three linear axes, which can be extended or combined to cover large workspaces, making them highly adaptable to various industrial applications. Additionally, their modularity allows for easy customization and scalability, enabling manufacturers to tailor the robot to specific tasks or workflows. These manipulators can be equipped with various end effectors, such as grippers, welding torches, or cameras, further expanding their functionality. Due to their precise control and adaptability, Cartesian manipulators are indispensable in modern manufacturing, delivering the precision and efficiency required for advanced automation and high-volume production environments.


# III. Jacobian Matrix

![1](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157590037/cc98c41d-665f-4e58-a3fd-28844857fbf7)
 ![Screenshot (544)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/d321bef9-df3b-48a0-bbb7-abecfaf3c84d)
![Screenshot (545)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/ac706bf2-ffd5-4005-92c6-69836592e793)
![Screenshot (546)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/2c44a569-d3f8-4854-8b9d-01b7b5796aa3)
![Screenshot (547)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/e103bc63-1b02-4976-8378-944551fc303c)
![Screenshot (548)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/a06c372f-2229-48fd-8ec7-077a168b2e2b)
![Screenshot (549)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/7c738d7a-4b92-4ab1-ac6e-a15eebde29b0)
![Screenshot (550)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/29d192ed-8590-4582-bfa0-0a9a4eeb2aff)
![Screenshot (551)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/c0331f9c-bd94-40c7-8d62-a75a4fb14002)
![Screenshot (552)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/bf9320f3-6dab-4b7e-9149-195f9c8ab7e5)
![Screenshot (553)](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157568463/4c6a112b-3eda-441c-b008-d324954f70bb)

## Click attached link to have access in the video

https://youtu.be/GvgBFPrsmmY

# IV. Differential Equation

The differential equation we got from our Jacobian Matrix is used to interpret or analyze the velocity of the end effector and joints of our mechanical manipulator.
Using this differential equations, we can identify how to change or adjust the velocity of the end effector in the x, y ,z axes as well as the rotation along x, y, and z axes. 
The differential equation of the velocity vector using the Jacobian matrix allows us to relate joint velocities to end-effector velocities, enabling precise control and analysis of robotic manipulators.
Geometrically, these configurations are determined, and they have practical implications in robot control and motion planning.

![Jacobian Matrix](https://github.com/billyabante/Robotics2_JacobianMatrix_Group15_Cartesian_2024/assets/157590037/458249b4-0992-480b-841c-94cf8c6f9ce7)

## Click attached link to have access in the video

https://youtu.be/q1Jp_M7wu0E

# V. Singularity

In robotics, a singularity is a particular configuration where the robot loses one or more degrees of freedom, making certain movements impossible or highly unpredictable. This happens when the robot's Jacobian Matrix, which connects joint velocities to the end-effector's velocities, becomes singular—its determinant reaches zero and it loses rank. At this stage, the end-effector might exhibit infinite velocities or erratic behavior with minimal changes in joint angles, complicating control and precision. Singularities can severely impact the stability, accuracy, and mechanical integrity of robots, making it essential to detect and avoid them in robotic design and operation.

**Here is the computation of the Cartesian Manipulator's Singularity**

![Screenshot (564)](https://github.com/billyabante/Robotics2_JacobianandPT_Group15_Cartesian_2024/assets/157568463/010538e5-2296-4025-b89c-1c2af98e4e65)

## Click attached link to have access in the video

https://youtu.be/-INU9u_6lQg

# VI. Path and Trajectory Planning

Define the robot's parameters: The user is prompted to input the link lengths a1, a2, a3, a4, and prismatic joint limits d1, d2, d3 in millimeters. These values are then converted to meters.

**Create the robot model:**
> A cartesian manipulator is created using the DHRobot and the Denavit-Hartenberg parameters. The robot consists of three prismatic joints. But 1 fixed joint is added and will serve as a stand.

**Define initial and target joint configurations:**
> The initial joint configuration q0 is set to an array of zeros. Three sets of target joint configurations q1, q2, and q3 are defined by the user input.

**Compute joint trajectories:**
> Joint trajectories are computed between the initial and target joint configurations using the jtraj function from roboticstoolbox. This function computes a joint trajectory with a specified number of waypoints (20 in this case) using a trapezoidal velocity profile.

**Plot the robot's motion:**
> The robot's motion is visualized using the plot method from the DHRobot class. The method displays the robot's motion over time, with the option to set limits on the x, y, and z axes. The robot's motion is plotted for each of the three target joint configurations.

![2024-05-2823-25-22-ezgif com-speed](https://github.com/billyabante/Robotics2_JacobianandPT_Group15_Cartesian_2024/assets/157590037/e607422d-250a-4cd2-8014-6bb639097683)

## Click attached link to have access in the video

https://youtu.be/FCCd5ClEV-I

<div align="center">
 
## VII. Cartesian GUI with Pick & Place and Welding

<div align="center">
  <a href="https://drive.google.com/file/d/1LD-3A2jJExdkl_EH9v0wCKQldzNiDTic/view?usp=sharing">
    <img height=100" src="https://github.com/billyabante/Robotics2_JacobianandPT_Group15_Cartesian_2024/assets/157665849/a0766921-caa1-4d51-9a65-9263c3792481"  />
  </a>
</div>
<div align="center">
Click here
