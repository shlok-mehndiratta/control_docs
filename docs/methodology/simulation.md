# Simulation Infrastructure (ROS 2)

## Rationale
A simulation environment allows rapid testing of control and vision algorithms without risking hardware damage.

## Environment Setup
We selected **ROS 2 Humble** because of:
- Strong communication architecture (Publish–Subscribe)
- Industry adoption
- Extensive community support

### OS Compatibility Challenge
ROS 2 Humble targets Ubuntu 22.04, but our systems included:
- Windows  
- Ubuntu 24.04  

This caused dependency failures.

### Solution: Docker
We standardized development using a Docker container based on Ubuntu 22.04.  
Benefits:
- Identical environments for all team members  
- No OS-specific issues  
- Simplified dependency management  

## Basic Control Prototyping (Turtlesim)
Before constructing a full drone simulation, we validated ROS fundamentals using Turtlesim.

### Safety-Cage Algorithm
- The bot moves in a circular pattern.  
- Its coordinates are monitored in real-time.  
- If the bot approaches within **2 cm** of the boundary, a high-priority turn command is issued.  

**Purpose:** Confirm understanding of ROS topics, publishers, subscribers, and feedback loops.

