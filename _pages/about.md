---
layout: about
title: about
permalink: /
subtitle: <a href='https://seee.hust.edu.vn/en/'> Control and Automaution Engineering / School of Electrical Engineering and Electronics (SEEE) </a>.
profile:
  align: left
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Hanoi, Vietnam</p>
    <div class="social-sidebar mt-3"> #addition
      {% include social.liquid vertical=true %} #addition
    </div> #addition

selected_papers: false # includes a list of papers marked as "selected={true}" #The original version is true, but i don't have any publish so turn off that function is necessary
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
    I'm an undergraduate at the <strong>Hanoi University of Science and Technology (HUST)</strong>, majoring in Control and Automation Engineering, with a research focus on intelligent control (Fuzzy Logic, Neural Networks) and dynamic optimization (MPC, Reinforcement Learning). My long-term interest is applying reinforcement learning and optimal control methods to autonomous systems and robotics.
  </p>
  <p>
    Most of my work lives at the intersection of theory and simulation. I've built and tested control strategies ranging from intelligent control to optimal control, working through the full loop of deriving dynamics, tuning controllers, and stress-testing them in MATLAB/Simulink before anything touches real hardware.
  </p>
  <p>
    I'm currently a Research Assistant at the <strong>Multi-Agent System Control (MASC) Laboratory</strong>, SEEE, HUST, supervised by Assoc. Prof. Hoai Nam Nguyen, where I work within a small team developing UAV flight control methods. My role centers on translating control theory into working implementations — designing and modeling controllers in MATLAB/Simulink, then validating and iterating on them through simulation, with Python for supporting analysis and scripting. I'm responsible for the modeling and controller-design side of the pipeline, working closely with teammates to refine and test results.
  </p>
  <p>
    Outside of research, I enjoy exploring controller design for quadrotors — from classical PID to self-tuning fuzzy and Lyapunov-based adaptive control — as a way to deepen my understanding of nonlinear control theory in practice.
  </p>
</div>
