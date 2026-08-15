# Chaitanya Belekar

<p align="center">
  <img src="./assets/hero.gif">
</p>

<p align="center">
  <a href="https://github.com/devwithchai">
    <img src="./assets/github-button.svg" alt="GitHub">
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/in/chaitanya-belekar/">
    <img src="./assets/linkedin-button.svg" alt="LinkedIn">
  </a>
  &nbsp;
  <a href="https://mail.google.com/mail/?view=cm&fs=1&to=chaitanyabelekar18@gmail.com">
    <img src="./assets/email-button.svg" alt="Email">
  </a>
</p>

---

## How I Build

I usually understand things better after trying to build them.

A derivation becomes clearer when it drives a simulation.  
A simulation becomes more interesting when it meets hardware.

That's the loop I keep coming back to:

**understand → build → break → improve → document**

---

## Currently Building

<table>
<tr>
<td width="50%" valign="top">

### OpenKinematics

A Python library for **robot kinematics, dynamics and visualization**, implemented from first principles.

Built mainly as a way to understand the mathematics behind robotics more deeply.

→ [View repository](https://github.com/devwithchai/OpenKinematics)

</td>
<td width="50%" valign="top">

### Mobile Robotics

Working with differential-drive robots, embedded controllers, sensors and ROS 2.

Moving from physical prototypes toward:

`odometry → sensor fusion → ROS 2 → autonomy`

→ [View repository](https://github.com/devwithchai/MobileRobotics)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Tendon-Driven Soft Robotic Finger

Exploring tendon-driven actuation, soft robotic mechanisms and dynamic simulation.

The current chain is:

`mechanism → actuation → modelling → simulation → control`

</td>
<td width="50%" valign="top">

### Digital Twins

Exploring how simulation, robot models and real-world data can come together to represent robotic systems.

</td>
</tr>
</table>

---

## Toolbox

Instead of a wall of badges, here's how the tools fit into the way I work:

| Layer | Tools I use | What they help me do |
|:--|:--|:--|
| **Code** | <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" height="25"/> <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white" alt="C" height="25"/> <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" alt="C++" height="25"/> <img src="https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white" alt="MATLAB" height="25"/> | algorithms, modelling, control |
| **Robot OS** | <img src="https://img.shields.io/badge/ROS 2-22314E?style=for-the-badge&logo=ros&logoColor=white" alt="ROS 2" height="25"/> <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" height="25"/> <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" height="25"/> | connect and develop robotic systems |
| **Simulation** | <img src="https://img.shields.io/badge/Gazebo-1E738A?style=for-the-badge&logo=gazebo&logoColor=white" alt="Gazebo" height="25"/> <img src="https://img.shields.io/badge/RViz-5A2E61?style=for-the-badge&logo=ros&logoColor=white" alt="RViz" height="25"/> <img src="https://img.shields.io/badge/MoveIt-5A2E61?style=for-the-badge&logo=ros&logoColor=white" alt="MoveIt" height="25"/> | test robots before hardware |
| **Hardware** | <img src="https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white" alt="Arduino" height="25"/> <img src="https://img.shields.io/badge/ESP32-E7342C?style=for-the-badge&logo=espressif&logoColor=white" alt="ESP32" height="25"/> <img src="https://img.shields.io/badge/Sensors-6E7D8C?style=for-the-badge" alt="Sensors" height="25"/> <img src="https://img.shields.io/badge/Actuators-6E7D8C?style=for-the-badge" alt="Actuators" height="25"/> | turn models into physical systems |
| **Design** | <img src="https://img.shields.io/badge/Fusion 360-1A8EBB?style=for-the-badge&logo=autodesk&logoColor=white" alt="Fusion 360" height="25"/> <img src="https://img.shields.io/badge/CAD-6E7D8C?style=for-the-badge" alt="CAD" height="25"/> | mechanisms and robot structures |

<details>
<summary><b>Current technical focus</b></summary>

<br>

`Robot Kinematics` · `Computer Vision` · `Control Systems` · `ROS 2` · `Robot Simulation` · `Embedded Robotics` · `Soft Robotics` · `Digital Twins`

</details>

---

## What I'm Exploring

I don't think of these as separate technologies. I'm interested in how they form one robotic system:

```mermaid
graph TD
    A[Perception]
    A_CV[(Computer Vision)]
    A_LIDAR[(LIDAR, IMU)]
    A --> A_CV
    A --> A_LIDAR

    B[State & World Model]
    C[Algorithms]
    D[Planning & Control]
    B --> C
    C --> D
    C_KD[("Kinematics & Dynamics")] -.-> C
    C_SLAM[("SLAM, Navigation")] -.-> C

    E[Simulation]
    F[Robot Hardware]
    E_DT[(Digital Twins)] -.-> E
    F_ES[(Embedded Systems)] -.-> F

    ROS2[("ROS 2")]

    A --> B
    D --> E
    E -- "Sim-to-Real" --> F
    F -- "Feedback Loop" --> A

    D -- "ROS 2 Msg" --> ROS2
    ROS2 -- "ROS 2 Msg" --> F

    %% Clickable links
    click C_KD "https://github.com/devwithchai/OpenKinematics" "View OpenKinematics repository" _blank
    click C_SLAM "https://github.com/devwithchai/MobileRobotics" "View Mobile Robotics repository" _blank
    click F_ES "https://github.com/devwithchai/MobileRobotics" "View Mobile Robotics repository" _blank
    click ROS2 "https://docs.ros.org/en/rolling/" "Go to ROS 2 Documentation" _blank

    %% --- Styling ---
    %% Define classes for each logical group
    classDef sense fill:#0077b6,stroke:#023e8a,color:#fff
    classDef think fill:#06d6a0,stroke:#073b4c,color:#000
    classDef act fill:#f9c74f,stroke:#f3722c,color:#000
    classDef orchestrate fill:#ef476f,stroke:#b22c49,color:#fff

    %% Assign nodes to classes
    class A,A_CV,A_LIDAR sense
    class B,C,D,C_KD,C_SLAM think
    class E,F,E_DT,F_ES act
    class ROS2 orchestrate
```

The interesting part for me is the loop:

**sense → understand → decide → simulate → act → learn**

That's where mathematics, algorithms, software and physical robotics start meeting each other.

---

## A Small Note

Not everything here is finished.

Some repositories are polished.  
Some are experiments.  
Some are ideas I'm still trying to figure out.

I prefer documenting the process rather than waiting until everything looks perfect.

---

<p align="center">

`< Keep building. Keep learning. Share everything. />`

</p>
