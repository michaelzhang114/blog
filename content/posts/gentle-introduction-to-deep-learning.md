---
title: "Introduction to Deep Learning"
date: 2019-12-09T22:40:19-05:00
draft: true
tags: [dl]
---

## Read this if you have:
------
- Basic computer programming knowledge
- Want to know what the hype is behind 'deep learning'

## Fundamentals
------

### DL vs. ML vs. AI

**AI**

To begin to understand deep learning, we must understand the difference between deep learning (DL), machine learning (ML), and artifical intelligence (AI).

Let's address artifical intelligence first. AI is intelligent behavior exhibited by computer programs. It can be as simple as using `if` statements. Take a look at the following code:

```java
var mainCharacter = new MainCharacter();
var enemy = new Enemy();

if (mainCharacter.isWalkingLeft()) {
    enemy.moveLeft()
} else if (mainCharacter.isWalkingLeft()) {
    enemy.moveRight()
} else {
    enemy.stayPut()
}
```

The enemy character moves left if the main character is moving left, moves right if the main character is moving right, and doesn't move otherwise. It's not very sophisticated, but it is a basic realization of AI.

**ML**

Stats

**DL**

Deep learning is machine learning on steroids. 

### Learning types

#### Supervised learning
Supervised learning is classification. A supervised learning model maps input to output data using provided input-output pairs.

ex. Take a set of emails, some are spam, and some are not (assume we know this for sure). Then, we can generate the following input-output pairs:
- `email1` -> `spam`
- `email2` -> `not spam`
- `email3` -> `not spam`
- `email4` -> `not spam`
- `email5` -> `spam`

We give these input-output pairs for the model to learn so when we show the model a new email, say `email6`, then it would output either `spam` or `not spam`. New emails are *classified* into categories.

#### Unsupervised learning
Unsupervised learning is reconstruction. An unsupervised learning model learns from no results. We provide the model with inputs without the labels so the model can develop a learning pattern and come up with its own classification.

#### Reinforcement learning
Reinforcement learning is decision-making. A reinforcement learning model automatically determines the ideal behavior within a specific context to maximize results. It's like training a dog. If a dog sits when you tell it to sit, you award it a treat. Over time, the dog learns that sitting when told is desirable because it gets rewarded. Through this reward system, the dog learns a new action.

#### Summary of learning types
- Supervised learning: 
  - Classification
  - `f(input)` -> `target`

- Unsupervised learning: 
  - Reconstruction
  - `f(input)` -> `likelihood`

- Reinforcement learning: 
  - Decision-making
  - `f(state, action)` -> `value`

## What is Deep Learning?
------

p34 of all slides showing how deep learning surpasses machine learning

Deep Learning is a class of machine learning algorithms that uses multiple layers to progressively extract higher level features from raw input.