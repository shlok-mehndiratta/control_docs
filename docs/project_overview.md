# Project Overview

## Introduction
This project aims to reproduce and extend the system proposed in the paper *“Aerial Vision-Based Guidance and Control for a Perception-Less Ground Vehicle”*.  
The core idea is simple:  
A drone acts as the “eyes” of a ground robot. The ground robot has no sensors and receives all navigation decisions from the drone.

## Core Components
1. **Vision Module**  
   Detects the UGV using ArUco markers and identifies road boundaries from an aerial camera feed.

2. **Control Module**  
   Computes steering commands based on visual error (offset from road center).

3. **Simulation Module**  
   Provides a safe virtual environment for testing UAV–UGV interaction before real-world experiments.

## Why This Matters
This approach is essential for environments where the ground robot cannot carry expensive sensing hardware or where remote supervision is required.

This website captures the full engineering process—from early prototypes to final implementation.

