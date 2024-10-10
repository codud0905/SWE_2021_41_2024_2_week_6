# Week 5 Assignment - Open-Source Software Practice

## Lecture Contents: Docker

### Task Description
The purpose: to set up an environment for a container.

This environment must meet the following requirements:
1. Linux OS
2. Git installed
3. Python3 installed
4. Bind mount

You need to create a container that satisfies the above conditions and demonstrate it.

### Tips & Specifications

#### Linux OS
- Use an image based on `ubuntu` (for example, `ubuntu` or `ossp` images).

#### Git & Python Installation & Check
- Run the following command to install Git and Python3:
  ```bash
  apt-get install -y git python3

---

# Week 4 Assignment - Open-Source Software Practice

## Lecture Contents: iPython (Google Colab)

### Task Description
1. Follow the Colab link and save a copy in your Google Drive
2. Write a Python code that solves the algorithm problem described below.
   
### Algorithm Task: Happy Number

#### Problem Description
Write an algorithm to determine if a number `n` is a happy number.

A **happy number** is defined by the following process:
1. Start with any positive integer.
2. Replace the number by the sum of the squares of its digits.
3. Repeat the process until the number equals 1 (where it will stay), or it loops endlessly in a cycle that does not include 1.
4. If the process ends in 1, the number is happy. Otherwise, it is not.

Return `True` if `n` is a happy number, and `False` if it is not.

#### Constraints:
- `1 <= n <= 2^31 - 1`

#### Example:
```python
def isHappy(n):
  save_num = set()
  while (n != 1) and (n not in save_num):
      save_num.add(n)
      digits = []
      for digit in str(n):
          digits.append(int(digit)**2)
      n = sum(digits)
  return n == 1
