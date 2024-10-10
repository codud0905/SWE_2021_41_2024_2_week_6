# Week 5 Assignment - Open-Source Software Practice

## Lecture Contents: Docker

### Task Description
The purpose of this assignment is to set up an environment for a container that will be used in the Open-Source Software Practice class. This environment must meet the following requirements:

1. Linux OS
2. Git installed
3. Python3 installed
4. Bind mount

You need to create a container that satisfies the above conditions and demonstrate it.

---

### Tips & Specifications

#### Linux OS
- Use an image based on `ubuntu` (for example, `ubuntu` or `ossp` images).

#### Git & Python Installation & Check
- Run the following command to install Git and Python3:
  ```bash
  apt-get install -y git python3
