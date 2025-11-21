# Month 01 – Development Log

## Scope of Work
This month focused on:
- Setting up infrastructure  
- Reviewing the base research literature  
- Establishing basic simulation and control logic  

## 1. Project Scope & Objective
We initiated development based on the paper:  
*Aerial Vision Based Guidance and Control for Perception-Less Ground Vehicles.*

### Goal
Create a cooperative UAV–UGV system where:
- The UGV has **no onboard sensors**
- The UAV provides all navigation cues using aerial vision

### Key Modules
1. **Vision Module** – UGV tracking and road detection  
2. **Control Module** – Steering command generation  
3. **Simulation Module** – Safe testing environment  

---

## 2. Visual Evidence (Placeholders)
Figure 1: *Initial autonomous boundary-checking logic using ROS 2 (Turtlesim).*  
Figure 2: *Early ArUco detection / line segmentation outputs.*

*Media will be added in later updates.*


### A. Simulation Infrastructure

#### Environment Architecture
Different team members used different OS versions (Windows, Ubuntu 24.04).  
But ROS 2 Humble supports only Ubuntu 22.04 → dependency conflicts.

#### Decision
Adopt Docker as the uniform development environment.

#### Outcome
Consistent builds, no OS issues, reproducible pipelines.

---

### B. Control Logic Prototyping
Using Turtlesim, we implemented a *Safety-Cage Algorithm*:
- Monitor the robot’s position  
- Trigger a turn when nearing the environment boundary  
- Validate ROS pub/sub understanding  

---

### C. Vision Development
Progress:
- Basic ArUco detection implemented
- Camera calibration started
- Preliminary line-detection tests run

Next Steps:
- Improve detection robustness
- Integrate with ROS
- Test with simulated drone feeds

