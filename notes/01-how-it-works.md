# Table of Contents

- [Intro](#intro)
- [How is image created?](#how-is-image-created)
- [Perspective projection](#perspective-projection)
- [Light and color](#light-and-color)
  - [Materials](#materials)
  - [Color](#color)

# Intro

this lesson focuses on a specific area of 3D computer graphics programming, which is 3D rendering.

particularly through the lens of the ray-tracing algorithm.

# How is image created?

<img src="./media/visualize-picture.png" alt="drawing" width="500px" style="display: block; margin-left: auto; margin-right: auto; margin-top: 20px; margin-bottom: 20px;" />

this conceptual slice is termed the **image plane**, akin to a canvas for artists.

3D objects are technically projected onto the image plane.

# Perspective projection

<img src="./media/project-object.png" alt="drawing" width="500px" style="display: block; margin-left: auto; margin-right: auto; margin-top: 20px; margin-bottom: 20px;" />

a technique that translates 3D objects into 2D images is known as **perspective projection**.

- creating an illusion of depth and space on a flat surface

imagine wanting to depict a cube on a blank canvas.

- the process begins by drawing lines from each corner/edge of the cube towards the viewer's eye.

- where each line intersects the image plane—a flat surface akin to a canvas or the screen of a camera—a mark is made.

**Question**: How to project objects like circles or something more complicated with no or a lot of corners/edges?

# Light and color

technique = shading

the color and brightness of an object within a scene are predominantly determined by how light interacts with the material of the object.

when photons encounter an object, they can be absorbed, reflected, or transmitted, with the outcome varying depending on the material's properties.

- however, a universal principle across all materials is the conservation of photon count: the sum of absorbed, reflected, and transmitted photons must equal the initial number of incoming photons.

- for instance, if 100 photons illuminate an object's surface, the distribution of absorbed and reflected photons must total 100, ensuring energy conservation.

## Materials

materials are broadly categorized into two types: conductors, which are metals, and dielectrics, encompassing non-metals such as glass, plastic, wood, and water.

- dielectrics are insulators of electricity, with even pure water acting as an insulator

- these materials may vary in their transparency, with some being completely opaque (not transparent) and others transparent to certain wavelengths of electromagnetic radiation, like X-rays penetrating human tissue

materials can be composite or layered, combining different properties.

- for example, a wooden object might be coated with a transparent layer of varnish, giving it a simultaneously diffuse and glossy appearance, similar to the effect seen on colored plastic balls

## Color

focusing on opaque and diffuse materials simplifies the understanding of how objects acquire their color.

the color perception of an object under white light, which is composed of red, blue, and green photons, is determined by which photons are absorbed and which are reflected.

the visibility of the object is due to the reflected red/green/blue (white light) photons reaching our eyes, where each point on the object's surface disperses light rays in all directions.

- however, only the rays that strike our eyes perpendicularly are perceived, converted by the photoreceptors in our eyes into neural signals

- al-Haytham's model of light perception
