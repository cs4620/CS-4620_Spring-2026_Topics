# CS 4620/8626 - Spring 2026 - Topics
These are the topics we are going to cover in class each day. Links to [example student videos ](https://www.youtube.com/playlist?list=PLH9qo0GKu2iQgPuzozltIuvLgEddxc43L) and [slides from class](https://uofnebraska-my.sharepoint.com/:f:/g/personal/17816140_nebraska_edu/IgCHg5Sr1POTT4uZ0xpYHfWsAcBjrFnqAThYk6a3sROkT3Y?e=5PhlNM)

<br/><br/>
---
---

# Day  -   - (🧑‍🏫Lecture)



## 💡New Idea:
- 

## 👩‍💻Code Together:
-

## 🧭Ideas to explore on your own
- 

## 🏁Final Code
- [The final code for today](https://github.com/cs2510/Fall2025.Day)
<br/><br/>
---
---



# Day 01 - January 13 - World Space [Blender] (🧑‍🏫Lecture 1)


## 🖼️Activity:
- Watch a film with heavy use of 3D Computer Graphics. (For example, consider [Rouge One](https://www.youtube.com/watch?v=kaAmF8gy6eQ) (start at 3:20?))
  - What kind of emotions is the director trying to evoke? 
  - How do computer graphics help us achieve that?
  
  <!-- ## Intro
  🏃‍♂️Seeing the world
  Bring pencil and paper
  Draw an orange w/o seeing the basketball
  Show the orange and draw basketball
  https://www.pexels.com/photo/orange-fruit-161559/
  https://www.youtube.com/watch?v=ItY5chvVZoA -->

## 💡New Idea: Fundamental problem of graphics
- Avagadro’s number
- We can never simulate at first principles, therefore everything has to be a simplification
- You can see example of this in a video that shows [meshes in Substance 3D Painter demo reel](https://www.youtube.com/watch?v=IOe154tJSQA) (up to :19)

## 👩‍💻Code Together: Create something in world space
- ::Video:: See the [city in Inception](https://www.youtube.com/watch?v=YoHD9XEInc0) (Start around 2:00)
- 🏃‍♂️Draw a city in Blender using cubes in world space.
- 🏀 Translate/Scale/Rotate
- 💡 x/y/z -> r/g/b
- 💡Moving windows in Blender
- 💡 n to bring out panels in Blender
- 💡 numbers to change view
- 💡 Apply changes
- 💡 Move pivot
- ⚠️ Laptops need to turn on emulation

## 💡New Idea: About Blender
- Blender v Maya v 3DSMax (ZBrush, Cinema 4D)
- What you can do in [Blender timelapse](https://www.youtube.com/watch?v=8VRtkdRPnos)

## 💡New Idea: Major Translations
-  How could you translate/scale/rotate in code?
-  Homogenous coordinates
-  Major Affine Transformation Matrices
   -  Translate:
      -  $\begin{bmatrix}0 & 0 & 0 & T_x\\0 & 0 & 0 & T_y\\0 & 0 & 0 & T_z\\0 & 0 & 0 & 1 \\\end{bmatrix}$
   -  Scale:
      -  $\begin{bmatrix}S_x & 0 & 0 & 0\\ 0 & S_y & 0 & 0\\0 & 0 & S_z & 0\\0 & 0 & 0 & 1 \\\end{bmatrix}$
   -  Rotation:
      -  Rotation based on this basic 2D rotation pattern:
      -  $\begin{bmatrix} cosine(\theta) & -sine(\theta) \\ sine(\theta) & cosine(\theta) \\\end{bmatrix}$
   -  Rotation about X:
      -  $\begin{bmatrix}1 & 0 & 0 & 0\\ 0 & cosine(\theta) & -sine(\theta) & 0\\0 & sine(\theta) & cosine(\theta) & 0\\0 & 0 & 0 & 1 \\\end{bmatrix}$
   -  Rotation about Y:
      -  $\begin{bmatrix}cosine(\theta) & 0 & sine(\theta) & 0\\ 0 & 1 & 0 & 0\\ -sine(\theta) & 0 & cosine(\theta) & 0\\0 & 0 & 0 & 1 \\\end{bmatrix}$
   -  Rotation about Z:
      -  $\begin{bmatrix}cosine(\theta) & -sine(\theta) & 0 & 0\\ sine(\theta) & cosine(\theta) & 0 & 0\\0 & 0 & 1 & 0\\0 & 0 & 0 & 1 \\\end{bmatrix}$

## 💡New Idea: Major Translations
- Left-handed v right-handed coordinate systems
