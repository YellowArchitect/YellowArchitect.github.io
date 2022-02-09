---
layout: post
title: "AR Capstone Project"
date: 2022-02-09
categories: site update
---

This post is about the capstone project I did at VT for my BA in CS (Computer Science).

To graduate from VT with a BA in engineering you need to work on what’s called a capstone project for a semester. These projects have you work on a team with other students where you have a designated client you work with to develop and have a working prototype of some tool or product. The project is meant to showcase all the skills you’ve developed as a student, including but not limited to teamwork, documentation and presentation, design, and relevant hard skills from your discipline.

For my capstone project I choose to focus on HCI (Human-Computer Interaction), specifically working on an AR mobile app meant to enrich guests’ experience while visiting Pamplin Historical Park near Petersburg, VA. Our goal was to help visiting highschoolers take more interest and get more out of the park. Working on the project with me was my fellow students Catherine Lee and Lauren Osborne, our instructor being Douglas Bowman.

The first thing we did was meet with our client and interested parties about the project to figure out what their vision was. This is when we learned that we were going to be focusing on something highschoolers would be using to engage with the park. For this reason, we decided that a mobile app would be the best platform to use. We also decided to use Unity game engine for development as it was what we were most comfortable working with, and we knew our school had extensive resources to help us along the way. We also decided on our project title, Pamplin P-AR-K.

We had a difficult start figuring out the concept of the app. We started with the idea of a treasure hunt or hide-and-seek, but when talking with our client decided it was too lighthearted. One of the main subjects that would be covered in the content of the app was slavery, and we wanted to treat the subject with as much respect as possible and not trivialize it. What we ultimately decided on was tracing the story of a fictional character, specifically a house slave’s diary. You would walk in the footsteps of the character following a digital map and interact with different AR objects. The final design would include relevant pictures, texts, and voiceovers describing the objects.

Two of the biggest hiccups we suffered were in actual implantation. We struggled to acquire a device that we could develop on, and I eventually decided to buy a Samsung Galaxy A52 5G. I was more familiar with android systems and needed to replace my old phone anyways, so the decision made sense to me. It also meant I could do development on my own time and guaranteed I would have a working device for the prototype on Demo Day, when we would present our final prototype to our instructor, students, and clients.

The other hurdle was how to implement the AR objects in the Unity engine world space. The original plan was to use GPS coordinates and the onboard compass to place the objects on the camera view in real time at the correct location relative to the user. Unfortunately, it turns out that GPS runs at low resolutions and mobile onboard compasses are also imprecise, so getting the exact relative coordinates for positioning the objects was essentially impossible. There would always be some level of rotational drift, or the object would appear several feet away from their correct coordinates. After tinkering with the code with no real results to show for it, we decided to change our method of showing the AR objects.

The solution we cam up with was using image recognition. For the demo day, we would be using a presentation to display what the location looked like since the demo wasn’t at Pamplin Park. I set up the software so that when a specific image was presented to the camera, an associated AR object would appear inside the image and could be interacted with. This was an imperfect solution, but it was a proof of concept. In the final implementation we would have to either use object recognition or use image recognition where we would take multiple photos at different angles and different times of day of the target location for the object. In practice you would follow the digital map and be instructed to show the camera the location when you get there, and voila! AR magic!

Even though we had a slow start and several technical hurdles, the project was ultimately a success. Our instructor and client were fairly impressed with the work we were able to accomplish in the relatively short amount of time we had to do it. Even though it wasn’t perfect, we still put on a good show on demo day and I’m proud of my team’s accomplishments. Catherine, Lauren, if you guys are reading this, I want to thank you guys for the great memories, hard work, and for pushing me when I felt like I was at a dead end. You guys are awesome, and I wish you the best.

If you want to look at what I did for the project, the repository can be found [here](https://git.cs.vt.edu/bensch/pamplin-p-ar-k/-/tree/master/Hello%20AR%20World), and some basic documentation can be found [here](https://docs.google.com/document/d/1GsYiHNEvye2AFMLmXLrCy3dYjvzf2ZLMrBvce86fiwM/edit?usp=sharing).

Sorry for the long post, but I hope it was interesting, enlightening, or just something different to think about. Cheers!
