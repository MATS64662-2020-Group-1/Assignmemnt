# Research Software Engineering Practice 2019-2020

This is the repository for the Research Software Engineering Practice module of the AMS CDT. 

## Aim of the Unit and of the Assignment

The aim of this course is to learn about modern software engineering practice, particularly to learn about Python, version control and collaborating on code development using the GitHub workflow.

As a group, a program to perform image-based physics (diffusion, thermal conduction, solid mechanics etc.) simulations should be developed using:

- Available open-source FE and image-analysis packages
- Microstructure images from your research work, scientific literature and/or the provided image database

This is an application of what has been covered in your Python and Git tutorials. The work should include documentation, examples and test cases with any further desired functionality added.

## First Task: Image Analysis

Assigned to: Joshua Collins

This task involves obtaining microstructural images from research work, scientific literature and/or the provided image database. It is important that full permission is acquired when using the images to avoid any copyright issues. The images will be pre-processed accordingly so they can be imported into an FE simulation e.g. through segmentation, mesh generation, removing speckle noise.

## Second Task: FE Processing

Assigned to: Sakina Rehman + Guy Bowker

This task involves using available open-source FE and image-analysis packages. The ‘cleaned’ image will be imported and using the generated mesh, assigned different material IDs/boundary conditions to different regions of the image. This highlights the importance of segmentation/mesh generation when pre-processing the image. From this, the packages will be used to create FE physics simulations e.g. deformation or heat flow in a composite.

Firstly, test cases will be created, which is a simple case where the solution is known (e.g. 1D heat conduction with a source at a known location) and compared to textbook/existing answers. If the solution is very different to the known solution, then it is clear that something is erroneous in the simulation. Each repository should have a suite of test cases to ensure the code is running as expected and to add a level of trust in the code. Each test case should be quick, easy to run and the solution should be clear. 

In terms of finding the FE packages, a simple Google search of ‘FE packages in Python’ can be done or skimage, http://sfepy.org/doc-devel/index.html, https://github.com/sfepy/sfepy can be used. Examples should also be created showcasing the project, using the available resources, and recreated for this project.
