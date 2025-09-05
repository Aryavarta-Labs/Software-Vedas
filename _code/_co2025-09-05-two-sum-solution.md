---
layout: post
title: "Two Sum Solution"
author: "Your Name"
categories: dsa
---

### Problem
Given an array of integers...

### Code (Python)
```python
def twoSum(nums, target):
    lookup = {}
    for i, num in enumerate(nums):
        if target - num in lookup:
            return [lookup[target - num], i]
        lookup[num] = i
