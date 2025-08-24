+++
date = '2025-08-23T14:45:13+05:30'
draft = false
title = 'Designing Portal in 2D - Exit Protocol'
tags = ['game dev', 'design']
+++

(1/2)

This post is part of a series of posts. This post discusses the **introduction** and **design** aspects of the game.

Click here for the 2nd post.

## Introduction

This summer, I got the opportunity to go to the National University of Singapore (NUS) and attend a course called 'The Structure & Interpretation of Computer Programs'. This course was an introduction to _programming methodology_, wherein we were supposed to understand basic concepts of programming and submit a final project towards the end.

Most people (including our team) decided to develop a game. After days of endless discussion as to what would be the most interesting and feasible idea, my team and I decided to develop a two-dimensional version of the popular game **'Portal'** as part of out project. The part about feasibility was of great importance, since the interesting part about working on this project was that we had to use a completely new language called **Source**. Luckily, this language was derived from JavaScript and didn't feel all that unfamiliar.

This course was 21 days long and all teams began their project work after the 11th day, as did we. To be honest, we were initially underconfident in our idea since:

- We didn't have any game development experience to begin with
- If you've ever played Portal before, you can guess that a crazy amount of physics would be needed to make it work
- We just learned about this new language 5 days ago AND it has its own modules and libraries!

Thankfully, the project turned out okay, better than we had imagined!

### Game concept

Exit Protocol is a 2D, puzzle based platformer game based on the popular game 'Portal'. In our version, the main character has to retrieve a keycard and bring it to the exit block in order to advance to the next level. The player can achieve this by creating a pair of portals! The player can enter one portal and exit the other one. Each new level is trickier than the previous one. Some levels contain buttons, doors, cubes etc. making the game more challenging and fun!

## Working with source

Source has its own libraries, which can be found [here](https://source-academy.github.io/modules/documentation/). Most people used the **arcade_2d** module, but due to its lack of support for physics-based functions, we ended up using the **unity_academy** module. This did pose some interesting challenges for us, for example, in portal, one can use the mouse cursor to aim where they want to shoot the portal. Since the unity_academy module did not support the detection of mouse-based inputs, we had to stick to keyboard inputs. I did consider pitching that we shift to arcade_2d on several occasions but decided against it since we had already worked on so much of the code in unity_academy.

## The Assets

### Main character

For the assets, we tried our best to make original designs. For the main character, I was inspired by a few Pinterest posts and a Winx Club character (Tecna), so I chose pink hair and green-blue eyes. I made the basic character art using a website called [Pixilart](https://www.pixilart.com/) and then had ChatGPT create a sprite sheet for it.

![player](/blog/docs/EP-player.png)

### Blocks & Background

The ground, exit & keycard blocks were pretty generic. Since Portal is set in a dystopian future, inside a testing facility which is similar to a lab, we decided to make greyish ground blocks. To set it apart, we decided to play around and make our version more cyberpunk. We actively utilised colours like shades of purple, blue, grey, orange and white throughout the design phase. Initially, we thought about making the game very black, white and grey, to make it seem more like a laboratory. We soon realized that this would make our game dull, and so we decided to lean into the cyberpunk aesthetic and added more colours to other blocks. Interestingly enough, some of these colours weren't just for a decorative purpose. For example, we added colour-coordinated buttons and doors to make the game a little harder to solve!

### UI - Help buttons and tutorials

We decided to keep this section simple and chose colors that would contrast with the background. Since the background was blue-green, white was a perfect fit. It took us a while to find the perfect shade of orange that would go with the background, but I'd like to think that we did a pretty good job with the color scheme overall!

![img](/blog/docs//posts/nus-sicp/img.jpg)

To learn more about the coding aspect, check out the [next post](https://coffeecookey.github.io/blog/docs/posts/nus-sicp/nus-sicp2/)!
