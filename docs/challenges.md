# Challenges & Solutions

This page tracks all major issues encountered during development and how they were resolved.

## 1. Operating System Mismatch
- ROS 2 Humble only supports Ubuntu 22.04.  
- Team used Windows + Ubuntu 24.04 → installation failures.  
**Solution:** Standardized with Docker.

## 2. Early Vision Instability
- Marker detection inconsistent under changing lighting.  
**Solution:** Added pre-processing filters; tuning continues.

