---
title: "Image Recognition API"
date: 2018-01-01
summary: "RESTful API for brand logo identification using a retrained Inception CNN"
tags: ["python", "go", "tensorflow", "flask"]
weight: 4
---

REST API for identifying brand logos in unlabeled social media photos, built with a retrained TensorFlow Inception V3 model.

Originated from a GapJumpers coding challenge — build a CNN that can identify Nike vs. Altra logos in untagged social media photos.

![Nike logo detection](/images/projects/NikeExample.jpg)
*Nike logo identified in social media photo*

![Altra logo detection](/images/projects/AltraExample.jpg)
*Altra logo identified in social media photo*

**How it works:**
- Transfer learning from Inception V3 to identify brand logos
- Flask API serving predictions
- Companion Go implementation of both the API and model inference

**Tech:** Python, Flask, Go, TensorFlow

[Flask version](https://github.com/chriskaschner/restful-api-flask) | [Go version](https://github.com/chriskaschner/restful-api-golang)
