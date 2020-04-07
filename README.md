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

## Third Task: Documentation

Assigned to: Frances Livera + Sam Lister

The code and examples should be documented correctly and clearly e.g. through using comment lines. It is not advised that a Word report is created as it will be seen as a binary file in GitHub and not as a gradual/updated document. Instead, in a Git repository, a text file can be created which can be marked up and changes can be seen clearly i.e. in pull requests. Latex is recommended as it is easier to manage on GitHub and easier to assess. There is no page limit for this report.

## GitHub Management and Collaboration

Assigned to: All group members

Grading is based upon how the project is managed, how the group collaborates on GitHub, how issues are raised and through pull requests. The quality of the technical job is not critical to the assessment.

When committing in the report, commits should show that the whole file has not just been committed, but instead frequently updated and approved by group members. Make sure the commit message is descriptive and try not to mix too many commits together. The commits should be atomic i.e. if a commit needs to be reverted, and only one functionality is causing an error, then the whole commit will need to be reverted regardless of whether the other functionalities within the commit caused an error or not. If commits are not atomic when reverting, then each functionality will need to be added separately, which is inconvenient. 

A set of commits that make up a functionality are known as features. Features should be created in separate branches and merged into a main branch. However, before merging, a pull request should be raised so that the group can review and approve of the pull request. If not, the changes will be biased.

Marks will be allocated based on the number and quality of your contributions as tracked by GitHub Pull Requests and by your participation in discussions, as recorded in Issues.
