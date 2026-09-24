# Flexbox Workshop

## Project Overview

This project demonstrates the use of CSS Flexbox to create a full-screen layout with six colored boxes. Each box has its own number and color.

The boxes are placed and animated through all nine main positions of the screen: Top Left, Top Center, Top Right, Middle Left, Center, Middle Right, Bottom Left, Bottom Center, and Bottom Right.

## Flexbox Properties Used

I used different Flexbox properties to control the position and arrangement of the boxes.

* **Justify-content** was used to control the horizontal position of the boxes, moving them to the left, center, or right.
* **Align-items** was used to control the vertical position of the boxes, moving them to the top, middle, or bottom.
* **Flex-direction** was used to control the direction of the Flexbox layout.
* **Flex-wrap** was used to allow the boxes to wrap when necessary.
* **Gap** was used to create space between the boxes.
* **Align-content** was used to control the arrangement of the Flexbox lines when wrapping was involved.

By combining the horizontal and vertical Flexbox properties, I was able to create all nine positions on the screen.

## Animation

I used CSS `@keyframes` to create an animation that automatically changes the Flexbox alignment. This allows the six boxes to move from one position to another without using JavaScript.

The animation is set to repeat infinitely, so after reaching the final position, it starts again and continues moving through the different positions.

## Animation Percentages

The percentages used in the animation represent different points on the animation timeline. They tell the browser when the Flexbox alignment should change during the animation.

I divided the animation timeline into different stages so that the boxes could move through all nine positions before the animation starts again.
For this project, approximately 9 stages are used so that the boxes can visit the 9 positions.

0%    → Top Left
11%   → Top Center
22%   → Top Right
33%   → Middle Right
44%   → Center
55%   → Middle Left
66%   → Bottom Left
77%   → Bottom Center
88%   → Bottom Right
100%  → Top Left again

The percentages do not represent screen positions.

They represent when a particular Flexbox position should occur during the animation.

🔢 Why 11%, 22%, 33%, etc.?

There are 9 positions that we want to demonstrate.

The animation timeline goes from:

0% to 100%

We divide this timeline into approximately equal sections so the boxes can move through the different positions.

For example:

0%     11%     22%     33%     44%
 |       |       |       |       |
 TL      TC      TR      MR       C

55%     66%     77%     88%     100%
 |       |       |       |        |
 ML      BL      BC      BR       TL

The final 100% returns the boxes to the starting position so that the animation can repeat smoothly.

## Video Demonstration

The video demonstrates the working Flexbox animation and explains how the different Flexbox properties are used to move the boxes around the screen.

##  Screenshots

The following screenshots show the six boxes moving through the nine Flexbox positions:

### 1. Top Left

![Top Left](screenshots/image1.png)

### 2. Top Center

![Top Center](screenshots/image2.png)

### 3. Top Right

![Top Right](screenshots/image3.png)

### 4. Middle Left

![Middle Left](screenshots/image4.png)

### 5. Center

![Center](screenshots/image5.png)

### 6. Middle Right

![Middle Right](screenshots/image6.png)

### 7. Bottom Left

![Bottom Left](screenshots/image7.png)

### 8. Bottom Center

![Bottom Center](screenshots/image8.png)

### 9. Bottom Right

![Bottom Right](screenshots/image9.png)


**Video Link:**
https://drive.google.com/file/d/1Bm26VWuBIjG0xeFTRMSsjx2nChIxuiBk/view?usp=sharing

## Technologies Used

* HTML5
* CSS3
* CSS Flexbox
* CSS Animation
* OBS Studio
