## Computer Graphics

### Week 1 - Introduction

#### Lecture 

Computer Graphics, the field of study used to create images / animations with a computer. In general terms: Digital modelling of 3D entities to synthetic images. 

**Scientific fields surrounding Computer Graphic**

1. Fields used by CG

   - Algorithms and Data Structures
   - Hardware architecture
   - Computational Geometry (algorithms for tasks with an immediate geometric interpretation)

2. Fields bounding CG

   - Computer Vision (robotic vision, in a sense, the inverse problem of CG)
   - Image Processing
   - Parallel Computing

3. Fields using CG

   - Interactive techniques (HCI - Human Computing Interaction)

   - Data Visualization

**Applications of Computer  Graphics**

1. Computational Biology: Computational biology is an interdisciplinary field that applies the techniques of computer science, applied mathematics and statistics to address biological problems. The main focus lies on developing mathematical modelling and computational simulation techniques.
2. Computational Physics: Computational physics is the study and implementation of numerical algorithm to solve problems in physics for which a quantitative theory already exists. It is often regarded as a sub discipline of theoretical physics but some consider it an intermediate branch between theoretical and experimental physics.
3. Information of Graphics: Information graphics or information graphics are visual representations of information, data or knowledge. These graphics are used where complex information needs to be explained quickly and clearly, such as in signs, maps, journalism, technical writing, and education. They are also used extensively as tools by computer scientists, mathematicians, and statisticians to ease the process of developing and communicating conceptual information.
4. Scientific Visualization: Scientific visualization (SciVis) is a branch of science, concerned with the visualization of three dimensional phenomena, such as architectural, meteorological, medical, biological systems. Scientific visualization focuses on the use of computer graphics to create visual images which aid in understanding of complex, often massive numerical representation of scientific concepts or results.
5. Graphic Design: The term graphic design can refer to a number of artistic and professional disciplines which focus on visual communication and presentation. Various methods are used to create and combine symbols, images and/or words to create a visual representation of ideas and messages. Graphic design often refers to both the process (designing) by which the communication is created and the products (designs) which are generated.
6. Computer-aided Design: Computer-aided design (CAD) is the use of computer technology for the design of objects, real or virtual. The design of geometric models for object shapes, in particular, is often called computer-aided geometric design (CAGD). CAD may be used to design curves and figures in two-dimensional ("2D") space; or curves, surfaces, or solids in three-dimensional ("3D") objects. CAD is also widely used to produce computer animation for special effects in movies, advertising, technical manuals.
7. Web Design: Web design is the skill of designing presentations of content usually hypertext or hypermedia that is delivered to an end-user through the World Wide Web, by way of a Web browser. The process of designing Web pages, Web sites, Web applications or multimedia for the Web may utilize multiple disciplines, such as animation, authoring, communication design, corporate identity, graphic design, human-computer interaction, information architecture, interaction design, marketing, photography, search engine optimization and typography.
8. Digital Art: Digital art most commonly refers to art created on a computer in digital form. On other hand, is a term applied to contemporary art that uses the methods of mass production or digital media. The impact of digital technology has transformed traditional activities such as painting, drawing and sculpture, while new forms, such as net art, digital installation art, and virtual reality, have been recognized artistic practices.
9. Video Games: A video game is an electronic game that involves interaction with a user interface to generate visual feedback on a raster display device. The electronic systems used to play video games are known as platforms. This platform creates through graphics.
10. Virtual Reality: Virtual reality (VR) is a technology which allows a user to interact with a computer-simulated environment. The simulated environment can be similar to the real world, for example, simulations for pilot or combat training, or it can differ significantly from reality, as in VR games. It is currently very difficult to create a high-fidelity virtual reality experience, due largely to technical limitations on processing power, image resolution and communication bandwidth. Virtual Reality is often used to describe a wide variety of applications, commonly associated with its immersive, highly visual, 3D environments.
11. Computer Simulation: A computer simulation, a computer model or a computational model is a computer program, or network of computers, that attempts to simulate an abstract model of a particular system.
12. Education: A computer simulation, a computer model or a computational model is a computer program, or network of computers, that attempts to simulate an abstract model of a particular system. Computer simulations have become a useful part of mathematical modelling of many natural systems in physics (computational physics), chemistry and biology, human systems in economics, psychology, and social science and in the process of engineering new technology, to gain insight into the operation of those systems, or to observe their behaviour.
13. Information Visualization: Information visualization is the study of the visual representation of large-scale collections of non-numerical information, such as files and lines of code in software systems, and the use of graphical techniques to help people understand and analyse data.

**General Pipeline**

In 3D computer graphics, the graphics pipeline or rendering pipeline refers to the sequence of steps used to create a 2D raster representation of a 3D scene. Plainly speaking, once a 3D model has been created, for instance in a video game or any other 3D computer animation, the graphics pipeline is the process of turning that 3D model into what the computer displays. 
$$
\text{Knowledge and data} \; \to (\text{modelling}) \; \to \text{Suitable representation} \; (\text{preprocessing modeling})\to \\(rendering/visualization)\;\to \text{Image(s)}
$$
Cultural Heritage
$$
\text{Real object} \;\to \text{3D polygonal mesh (Semplification, filtering..)}\;\\\to (rendering) \to \text{Images (Museum kiosk)}
$$
Games
$$
\text{Artist (content creator)}\to \text{Manual modeling (Maya, Blender...)}\to \\ \text{Polygonal mesh + texture(Simplification, UV mapping,rigging)}\to (rendering)\to \text{Images}
$$
SciViz Analysis of Earthquake
$$
\text{Math model of the quake} \to  (physical\;simulation)\to \text{Scalar field (time varying)} \to \\ (various \;processing\;ops\;(ex.color-coding)) \to (visualization) \to \text{Images}
$$
**The other main Approach**
$$
\text{3D Scene}(Made\;of\;rendering\;primitives) \to (rendering)\to \\ \text{Images}(raster\;images: 3\;channel\;RGB\;and\;8\;bits\times channel)
$$
**Human Visual System and Camera**

![1555805185610](C:\Home\notes\uts\Computer Graphics\computer-graphics.assets\1555805185610.png)

**Pin Hole Camera** : A pinhole camera is a simple camera without a lens but with a tiny aperture, a pinhole – effectively a light-proof box with a small hole in one side. Light from a scene passes through the aperture and projects an inverted image on the opposite side of the box, which is known as the camera obscura effect.

![Image result for pinhole camera](C:\Home\notes\uts\Computer Graphics\computer-graphics.assets\science-behind-camera-obscura.gif)

**Ray casting**: Raycasting  is a rendering technique to create a 3D perspective in a 2D map. Back when computers were slower it wasn't possible to run real 3D engines in real-time, and raycasting was the first solution. Raycasting can go very fast, because only a calculation has to be done for every vertical line of the screen. Ray casting is capable of transforming a limited form of data into a three-dimensional projection with the help of tracing rays from the view point into the viewing volume. 

The main principle behind ray casting is that rays can be cast and traced in groups based on certain geometric constraints. In ray casting, a ray from the pixel through the camera is obtained and the intersection of all objects in the picture is computed. Next, the pixel value from the closest intersection is obtained and is further set as the base for the projection. Ray casting is distinct from ray tracing, with ray casting being a rendering algorithm which would never recursively trace secondary rays, while ray tracing is capable of doing so. Ray casting is also simple to use compared to other rendering algorithms such as ray tracing. 

![1555808374302](C:\Home\notes\uts\Computer Graphics\computer-graphics.assets\1555808374302.png)

Idea $\to$ Follow back the light beams that come to the observer. For every pixel on screen: send a ray on screen (the primary ray from that pixel) and find its 1st intersection with an object in the scene.

```
for each pixel p
	make a ray r (viewpoint to p)
	for each primitive o in scene:
		find intersect(r, o)
		keep closest intersection oj
		find color of oj at p
```

Based on ray-primitive intersection (highly-optimized). Easy to compute: cast shadows (sharp) 

**Ray tracing**: In computer graphics, ray tracing is a rendering technique for generating an image by tracing the path of light as pixels in an image plane and simulating the effects of its encounters with virtual objects.  This is same as ray casting but ray bounces multiple times. Specular reflections (multiple too) and semi transparency with refraction are easy to compute. 

To determine a colour, for say the pixel, a ray tracer constructs a mathematical ray that starts at the camera, crosses the centre of the pixel, and then extends off into the scene. Kind of like a laser beam pointer at the pixel but from the camera. The ray tracer computes the closest intersection point between the scene objects and that ray. It then determines the colour of the intersected object at that point, and paints the picture that colour. This process is done for all of the pixels in the image. 

```
for each pixel p:
	make a ray r (from viewport to p)
	while(...)
		for each primitive o in scene:
			find if intersect(r,o)
			keep closest intersection
			r = new_bounce(r);
			find color from p (according to all paths)
```

Advantages of ray tacing

- Conceptually simple algorithm
- Takes into account Global effects
- More realistic rendering of lighting effects
- More freedom of primitives (intersect easier than project + rasterize)
- Potentially great scalability with scene complexity



**Rasterization**: Rasterization is the task of taking an image described in a vector graphics format (shapes) and converting it into a raster image (A series of pixels, dots or lines that when they come together on a display, they recreate the image). Also known as Transform and Lighting (T&L). Rasterization may refer to either the conversion of models into raster files, or the conversion of 2D rendering primitives such as polygons or line segments into a rasterized format. This is typically a process of identifying the needs of a specific media configuration, then allocating resources so that images are efficiently and optimally projected on the display device.
$$
\text{vertices 3D} \to(transforpm)\to \text{triangle 2D on screen}\to(rasterize)\to\\\text{fragments aka pixels}\to (fragment\;process)\to \text{output image}\;
$$
All operations are massively parallelizable.

Rendering primitives in rasterization: 

![1555811862804](C:\Home\notes\uts\Computer Graphics\computer-graphics.assets\1555811862804.png)

```
/* Raycasting */
for each pixel p:
	make a ray r
	for each primitive o in scene
		if intersect(r,o)
		then find color for o
			color p with it

/* Rasterization */
for each primitive o:
	find where o falls on screen 
	rasterize 2D shape
	for each produced pixel p:
		find color for o
		color p with it
```

Advantages of rasterization:

- More easily parallelizable
- More controllable complexity
- Better-suited for graphics cards (for now)
- Easier with dynamic data
- Better treatment of anti-aliasing (more later on)
- Better scalability with image resolution



**Rasterization s Ray tracing**

| Ratserization                                                | Raytracing                                                   |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![1555815028506](C:\Home\notes\uts\Computer Graphics\computer-graphics.assets\1555815028506.png) | ![1555815016280](C:\Home\notes\uts\Computer Graphics\computer-graphics.assets\1555815016280.png) |
| $\text{for each primitive}$<br />       $\text{for each pixel}$ | $\text{for each pixel}$<br />     $\text{for each primitive}$ |
| Fast (for each primitive, process only a few pixels instead of: for each pixel, process all primitives) | Good for complex visual effects. Shadows, specular reflections, refractions, .. |
| SW-based (CPU)                                               | HW-based (GPU)                                               |
| Off-line, hi quality renderings                              | Real time, compromise quality renderings                     |



#### Coding Session - Three JS Basics

```javascript

```

###  Week 2 - The Transform Phase

#### Lecture



#### Coding Session - Three JS Basics

```javascript

```



### Week 3 - Geometric Transformations

#### Lecture



#### Coding Session

### Week 4 - Lighting

#### Lecture



#### Coding Session

### Week 5 - Shading

#### Lecture



#### Coding Session

### Week 6 - 3D Models

#### Lecture



#### Coding Session



## Quiz One

1. Is the following characteristic of Ray Tracing or Rasterization? - Needs intersection ray primitive function: (  **Ray Tracing** -- Rasterization)

2. Is the following an example of Scientific Visualization or Information Visualization? - Visualize CT Scan dataset (**Scientific Visualization** -- Information Visualization)

3. Is the following an example of Scientific Visualization or Information Visualization? - Interaction Between football players (Scientific Visualization -- **Information Visualization**)

4. After computed the View coordinates have been computed, what is the MINIMAL information needed to compute the view frustum? (Position of the camera, Direction of view -- Position of the camera, Near clip, Far clip -- Near clip distance, **Far clip distance, width and height of View Volume**)

5. Is the following true for Object Coordinates or World Coordinates? - Is the reference frame of a 3D scanned object (**Object Coordinate** -- World Coordinates )

6. Given an object lying horizontally whose barycentre is (x0,y0,z0) in object coordinates. how do I bring the object vertically in position (x1,y1,z1) ?  (move by   (-x1,-y1,-z1), then Rotate by 90 degrees then move by (-x0,-y0,-z0) ----- **move by   (-x0,-y0,-z0) then Rotate by 90 degrees  then move by (x1,y1,z1)** --- move by   (-x1,-y1,-z1), then move by   (-x0,-y0,-z0) then Rotate by 90 degrees )

7. Given a 4x4 matrix encoding affine transformations T0,T1 (Translation) ; R0,R1 (Rotations) ; S0,S1 (Scaling). The resulting matrix R0 ∙T0 ∙ S0  (where ∙ is matrix multiplication) performs:  (**Rotate then Translate then Scale** ---Scale then Translate then Rotate)

8. Given a quad if I apply an affine transformation tf may become a rectangle. (True and **False**)

9. R0 ∙T0 is equivalent to T0 ∙ R0 (True -- **False**)

10. Given a Phong Material with High specularity which among the 3 view-Points will perceive the point P with more light incoming?

    ![1555121138578](C:\Home\notes\uts\CG\computer-graphics.assets\1555121138578.png)

    (all the same - 1- -2 --**3**)

11. Every Material has its own BRDF (**True** or False)

12. Given a Lambertian material which among the 3 view-Points will perceive the point P with more light incoming? (**All the same** -- 1-- 2 --3)

    ![1555121173707](C:\Home\notes\uts\CG\computer-graphics.assets\1555121173707.png)

13. What does the Phong shading NOT need? (**Normal per Vertex** -- Normal per Face -- Normal per Fragment)

14. What is the problem of Phong and Gouraud Shading with respect to FLAT shading?  (Lack of realism -- Inefficiency on representing smooth surfaces  -- **Need some extra data to represent sharp features** -- Impossible to represents sharp feature)

15. What does the FLAT shading need? (Normal per vertex -- **Normal per Face** -- Normal per Fragment)

16. 