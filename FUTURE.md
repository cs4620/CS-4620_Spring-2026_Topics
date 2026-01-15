# Day 28 - April 30 - Ray Tracing 6 [CPU] (🧑‍🏫Lecture 16)
# Day 27 - April 28 - (👟Sprint)
# Day 26 - April 23 - Ray Tracing 5 [CPU] (🧑‍🏫Lecture 15)

Shader Toy
Ray Tracing on the GPU (not RTX): https://www.shadertoy.com/view/tl23Rm 

# Day 25 - April 21 - (👟Sprint)

# Day 24 - April 16 - Ray Tracing 4 [CPU] (🧑‍🏫Lecture 14)

## Watch Sea Hawk sword fight and look at shadows

## Look at Snow White and see when there are and are not shadows

## Add shadows
- Check in the diffuse loop if there is a collision
- Resolve issue where we have self-collisions

# Day 23 - April 14 - (👟Sprint)

# Day 22 - April 09 - Ray Tracing 3 [CPU] (🧑‍🏫Lecture 13)

## Talk about shadow maps
Contrast to ray tracing

## Add Lights

## Moved to normalized lighting
- Instead of hard-coded rgb(r, g, b), store lighting at [0, 0, 0]

## Add diffuse lighting
- For each light, calculat the dot product and add to the accumulated light

## Double sided triangles
(I should probably have figured out winding order by now)

## Abstract out ray casting
- Create a CastRay function

Watch some Frozen to look for ray tracing

# Day 21 - April 07 - (👟Sprint)

Rotating around an origin


# Day 20 - April 02 - Ray Tracing 2 [CPU] (🧑‍🏫Lecture 12)

## Add multiple triangles to a list with colors

## Handle multiple triangles when ray tracing

## Definition of a circle

## Collision math with a circle

## Implement Circles

# Day 19 - March 31 - (👟Sprint)

# Day 18 - March 26 - Ray Tracing 1 [CPU] (🧑‍🏫Lecture 11)

Ray Tracing 1 (Ray trace a triangle. How to find a pixel’s location in space. How to collide with an infinite rectangle)
Cars 1 Trailer - https://www.youtube.com/watch?v=pQly7_Cj34U

## Theory of Ray Tracing

## Ray directions

## Plane intersections

## Triangle inside test

# Day 17 - March 24 - (👟Sprint)

# Holiday - March 18 - (Class Canceled)

# Holiday - March 16 - (Class Canceled)

# Day 16 - March 12 - Rasterizer 5 [GPU] (🧑‍🏫Lecture 10)

Shadow Maps?

# Day 15 - March 10 - (👟Sprint)

# Day 14 - March 05 - Rasterizer 4 [GPU] (🧑‍🏫Lecture 9)

Start with code from previous week

## Add multiple frames

## Clearing the color

## Z Buffer and clearing the Z Buffer

## Adding normals and uvs

## Passing normals and uvs

## Passing from vertex to fragment shaders

## Diffuse shading

## Adding more triangles


OBJ Files
Parsing obj files
OBJ v FBX v USD
https://www.pixar.com/usd

# Day 13 - March 03 - (👟Sprint)

# Day 12 - February 26 - Rasterizer 3 [GPU] (🧑‍🏫Lecture 8)

  ## Review
  - What is the perspective matrix?
  - How does it work

  History of GPUs (Silicon Graphics, DirectX, id)
  Reviewed what a GPU is and its parallelism
  OpenGL v DirectX v Vulkan v Metal
  HLSL v GLSL v WGSL
  Reviewed webgl starter code.
  

  ## Setting up the webgl context

  ## Setting up the position vertices, modelViewMatrix, and projectionMatrix

  ## Setting up the variables on the vertex shader

  ## Indexed vertices

  ## Drawing


  More recently, I wrote OpenGL from scratch, but kept a file with the webgl boiler plate that I needed to finish it.


# Day 11 - February 24 - (👟Sprint)


# Day 10 - February 19 - Rasterizer 2 [GPU]  (🧑‍🏫Lecture 7)

<!-- - Toy Story Trailer v Cars Trailer

  GPU v CPU – Renderman Intro https://vimeo.com/568471200
  Example Shader code from Renderman - https://renderman.pixar.com/stories/stylization-at-pixar -->

  ## Cover projection matrices

  ## In shader frog, implement custom projection matrix

  Major Matrix transforms
  ModelView v Projection
  1.	Unilluminated Shader: https://shaderfrog.com/app/view/3149?view=shader
  a.	GLSL (v HLSL)
  b.	Uniforms
  c.	Attributes
  d.	Matrices
  e.	Vertex Shader
  i.	gl_Position “return” value
  f.	Fragment Shader
  i.	gl_FragColor “return” value
  ii.	0-1 instead of 0-255
  iii.	vec4
  2.	Unilluminated Shader w/ variable (uniform) https://shaderfrog.com/app/view/3150
  a.	Fragment Shader
  i.	Set the precision of the float values
  ii.	Uniform variable
  iii.	vec3 to vec4
  3.	Normal Shader: https://shaderfrog.com/app/view/3151
  a.	Transfer additional information between fragment and vertex shaders
  b.	Vertex Shader
  i.	Get additional normal data
  ii.	“return” additional normal data
  iii.	We apply the world matrix and normalize it
  c.	Fragment Shader
  i.	Gets normal data (varying)


  4.	Diffuse Shading Only: https://shaderfrog.com/app/view/3152?view=shader
  a.	Fragment
  i.	Get uniform for directional light
  ii.	Diffuse calculation
  5.	Diffuse + Ambient Shading: https://shaderfrog.com/app/view/3153
  6.	Point Light (World Space Light): https://shaderfrog.com/app/view/3154
  7.	Dynamic (Time-based) Fragment Shader: https://shaderfrog.com/app/view/3155
  8.	Dynamic (Time-based) Vertex Shader: https://shaderfrog.com/app/view/3157
  9.	UV Shader: https://shaderfrog.com/app/view/3156
  10.	Grid UV Shader: https://shaderfrog.com/app/view/3158
  11.	Vertex Distortion Based on UVS: https://shaderfrog.com/app/view/3159
  12.	Vertex Distortion Based on UVS (non-uniform): https://shaderfrog.com/app/view/3219
  13.	Christmas “Ornament” using fragment and vertex shaders: https://shaderfrog.com/app/view/3221


# Day 09 - February 17 - (👟Sprint)

 - Inverse kinematics
  - Highlights on eyes
  - Proportional editing
  
# Day 08 - February 12 - Rasterizer 1 [GPU] (🧑‍🏫Lecture 6)

## Renders in Blender
  - How to render
  - How to align the camera with the view
  - How long would it take to render an animation?

  ## Rasterizing v Ray Tracing v Hybrid
  - Show Blender rendering a glass sphere
  - Show Cornell box
  - Show NVIDIA diagram

  ## Bias v Unbiased

  ## GLSL v HLSL

  ## GLSL in Shader Toy
  - Simple one-color shader


# Day 07 - February 10 - (👟Sprint)

# Day 06 - February 05 - Animation [Blender] (🧑‍🏫Lecture 5)


## Review
  Dot Product Questions

  ## History
  Disney and animation
  - Disney Springs Animators Picture
  - Pins
  - Dope sheets
  - Key frames
  - Tweeners

  ## Class Activity
  Animate a scene from Star Wars
  - https://www.youtube.com/watch?v=ykXWRNZiI3M
  - Timeline
  - Dope sheet
  - Frames
  - Keyframes
  - Go to frame - Make a change - Set a key frame
  - Graph editor


  ## Math 
  Interpolation
  Given a value at frame S and frame E, interpolate to find the value at frame F

   ## Review
  Given a value at frame S and frame E, interpolate to find the value at frame F

  ## Kinds of renderers
  Rasterizers v Ray Tracers

  Rigging
  Animation 2
  Rigging/Armatures
  Creating actions in Blender
  Animation using parents and children
  Watched Empire Strikes Back walkers scene to talk about go motion
  Watched Jurassic Park talk about soft-body animation
  Finding Dory - https://www.youtube.com/watch?v=Nn0S2vmSCU0


# Day 05 - February 03 - (👟Sprint)

## Review Questions
  Create a translation matrix
  Create a scale matrix
  What is a dot product
  What is a cross product
  What is a normalized vector
  What is ambient light
  What is diffuse light
  What is specular light
  What is a normal
  What is a uv


# Day 04 - January 29 - Shading 2 [Blender] (🧑‍🏫Lecture 4)

 ## Review
  Do a quick cross product question

  ## Sprint Review

  ## Math Starter
  - Normalize vectors
  - Interpolate normals across a triangle

  ## Interpolate normal
  Barycentric coordinates
  - See calculator


  ## Texturing
  Wrapping paper
  Activity: Wrapping paper

  Wrapping maps
  Activity, Reviewing mapping projections

  Look at the Wolfenstein 3D

  ## Blender UV Activity
  - Look at the UV maps for a sphere
  - UV map projections
  - Save UV map outlines for space ship

  ## Actual texture maps
  - See head texture map

  ## Weight painting in blender

  ## Professional software
  Substance 3D
  Activity: Review Substance 3D demoreel/website

  <!-- ## Normal maps -->

# Day 03 - January 27 - Shading 1 [Blender] (🧑‍🏫Lecture 3)

? Talk about cross product to do extrusion?

  ## Math Review
  Do a dot and cross product
  See Today for websites with tools

  ## What is Shading



  ## How light reflects
  Atomic level
  BSDF ideas
  - Diffuse
  - Specular
  Ambient Light

  ## Why don’t you tan in the winter

  ## Kinds of lights in a scene
  - Point
  - Spot (turn up wattage in Blender)
  - Sun
  - Area

  ## Shading in Blender
  - Different shading views in main view
  - Changing ambient light in the world tab
  - Adding a material to a mesh

  ## Shader tab in Blender
  - Visual scripting
  - Pins and wires
  - Add ambient, diffuse, and specular (glossy) shaders

  ## Normals on Objects
  - Different kinds of shading in Blender (smooth v flat)


  <!-- ## Normal maps
  •	In Blender:
  Create a high-poly and low-poly mesh. 
  •	Add details to the high-poly mesh
  •	Add a shader to the low-poly mesh.
  •	Create and select an image texture in that shader
  •	Chane renderer to cycles
  •	Open bake tab.
  •	Change from Combined to Normal
  •	Select selected to active
  •	Set Extrusion to 1m
  •	Bake -->


  <!-- ## OBJs -->

  <!-- ## Example
  Professional Shaders – Pixar – https://vimeo.com/568462499 -->


