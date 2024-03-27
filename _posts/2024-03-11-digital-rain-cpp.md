---
layout: post
title: "Digital Rain Project"
tags: cpp programming digital-rain matrix
categories: project
---

In this blog post, I'll unravel the workings of these four main methods, alongside the supporting functions that bring this digital rain project to life.

## Matrix Screen:

<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/matrixScreenCode.png" width="400" height="300">

The matrix screen function is the heart of my digital rain project. It initializes a sequence of characters that rain down the screen, creating the iconic Matrix effect. This method accomplishes its task by generating a new line of random characters for each column where a switch is active. These switches are Boolean values that determine whether a character should be displayed or not, providing an ever-changing rain pattern.

The function begins by resizing the switches array to match the width of the screen, ensuring that each column has its associated switch. It then enters a loop, where for each iteration, it generates a new string of characters – creating a line of the Matrix. If a switch for a given column is turned on, a character is placed; otherwise, a space is added, simulating gaps in the rain. This pattern is then inserted at the beginning of a vector that stores all lines, simulating the rain effect as it cascades down the screen. To maintain the illusion of movement, the oldest line is removed once the vector exceeds the console's height, ensuring that the rain never overflows the screen's boundaries.


<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/Matriximg.png" width="400" height="300">

## Reverse Colour Rain:


<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/reverseRainColourCode.png" width="400" height="300">

The reverse colour rain function introduces vibrancy to the Matrix rain effect by alternating the colors of the characters. Leveraging the `setTextColor` function, it assigns a unique color to each column based on its index, creating a rainbow-like appearance amidst the digital rain. This method follows a similar logic to the matrix screen, with the addition of color manipulation to enrich the visual experience.

As with the matrix screen, it utilizes the switches array to control the display of characters, turning them on and off randomly to mimic the erratic nature of rain. The primary distinction lies in its colorful presentation, offering a more visually dynamic and appealing version of the Matrix effect.

<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/reverseRainColourimg.png" width="400" height="300">

## Square Screen:


<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/squareScreenCode.png" width="400" height="300">

The square screen function introduces geometric shapes into the digital rain. By randomly positioning squares filled with characters across the screen, it adds an element of structural complexity to the visual output. This method involves generating a square by selecting a random starting point within the screen's dimensions and then filling the designated area with random characters, creating a solid square shape.

After displaying the square, the entire screen is cleared, and the process repeats, with the square moving downwards to simulate falling. This continual regeneration and movement of squares offer a unique take on the digital rain concept simulting raindrops falling on the screen.


<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/Squarescreenimg.png" width="400" height="300">

## Heart Screen:
<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/HeartScreenCode.png" width="400" height="300">

The heart screen function adds a twist to the digital rain, drawing heart shapes. Utilizing the `drawHeart` function, it places a heart pattern onto the screen, filled with characters for added effect. This method showcases the flexibility of the digital rain concept but also introduces a personal element to the project.

As with the square screen, the heart patterns are generated at random positions and fall down the screen, creating a display of digital affection. The use of color further enhances the visual appeal, painting the hearts in shades of pink.

<img src="https://raw.githubusercontent.com/Mugbo/digital-rain-cpp/main/docs/assets/images/heartimg.png" width="400" height="300">

## Supporting Functions:

Integral to the operation of these main methods are Supporting functions like `randomChar`, which generates the characters used in the rain; `setTextColor`, which manipulates the color output; and `drawHeart`, a function for crafting heart shapes within the digital rain. Each plays a crucial role in bringing the project to life, providing the necessary tools to create the rich and dynamic visual experience.

In conclusion, my digital rain project goes beyond the traditional Matrix effect, introducing variations that captivate. Through the design of each function, I have created a versatile and visually stunning application that puts a twist on digital rain while ustilizing my creativity.



