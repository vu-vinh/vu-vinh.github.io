---
# using "<div style="overflow: hidden; display: block;">" make the text won't spread in profile picture field, this is my personal change
# change the "allign:" from "right" to "left"
# change the "title" to upper character, this is my personal change
# The original version of "selected_papers" is true, but i don't have any publishs so turn off that function is necessary
layout: about
title: About
permalink: /
subtitle: # <a href='https://seee.hust.edu.vn/en/'> Control and Automaution Engineering / School of Electrical Engineering and Electronics (SEEE) </a>.
profile:
  align: left
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Department of Automation</p>
    <p>School of Electrical and Electronics Engineering, HUST</p>
    
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---
<div style="overflow: hidden; display: block;">
  <!-- This is an addition, not the original version. It solved the problem that the picture is floating so the content will overflow in the picture's field -->
  <p>
    I'm an undergraduate at <strong>Hanoi University of Science and Technology (HUST)</strong>, majoring in Control and Automation Engineering, with a research focus on modern control theory for robotics, spanning both optimal control (Model Predictive Control, and — going forward — reinforcement learning and deep reinforcement learning) and intelligent control (direct adaptive fuzzy control and deep neural-network-based control). My long-term interest is applying optimization-based and learning-based control methods to autonomous robotic systems.
  </p>
  <p>
   Most of my work lives at the intersection of theory and simulation: deriving nonlinear system dynamics, designing controllers around them (from decoupled MIMO MPC formulations to state-augmented adaptive laws), and validating performance in MATLAB/Simulink — with Python for supporting analysis. I'm looking to grow this further by bringing RL/DRL into my optimal control work and deep neural networks into my intelligent control work.
  </p>
  <p>
    I'm currently a Research Assistant at the <strong><a href='https://seee.hust.edu.vn/vi/nghien-cuu/macs/'>Multi-Agent System Control (MASC) Laboratory</a></strong>, SEEE, HUST, supervised by <a href='https://seee.hust.edu.vn/en/con-nguoi/nguyen-hoai-nam/'>Assoc. Prof. Hoai Nam Nguyen</a>, where I work on control algorithms for robotic systems within a small team, currently centered on UAV flight control. My role centers on the modeling and controller-design side of the pipeline — building plant models, configuring and debugging MPC blocks, and implementing adaptive/learning-based control laws — working closely with teammates on validation and testing.
  </p>
  <p>
   Outside of research, I enjoy exploring controller design more broadly across robotic platforms — from classical PID to self-tuning fuzzy and Lyapunov-based adaptive control — as a way to deepen my understanding of nonlinear control theory in practice.
  </p>
</div>
