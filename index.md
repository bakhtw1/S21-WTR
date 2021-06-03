# Work Term Report W21

School of Computer Science
3D Models and 3D Web Visualisation Canada - 3D Support
Winter 2021

## About

This blog details the experiences I had during my work term spent as a Research Developer at the Geological Survey of Canada at Natural Resources Canada. This was a time in my career where I was introduced to many new and challenging concepts, and has been the greatest learning experience for me to date. 

## Natural Resources Canada

Natural Resources Canada (NRCan) is a department of the federal government that deals with scientific research in various fields regarding Canada’s resources, geography, and more.  The branch I was working is was the Geological Survey of Canada, where we do various mapping/measurements of the geography of Canada. My supervisors were scientific researchers who were working on machine learning models for creating the massive 3D models that I was working on. I only interacted with my direct supervisor and manager, but only because of the online nature of the internship.


## Job Description

This co-op term was unique from other terms, in the sense that it was research heavy and mostly independent work. My job was to build upon work done by a previous student where we were testing two different GIS platforms that had support for streaming massive 3D geological models over the web. A solution for efficiently viewing massive 3D models in the web is to convert them into a hierarchical level of detail (HLOD) format. This format is usually a tree data structure, in our case we used a Octree. While the previous student worked mostly on converted surface meshes (hollow models, only surface represented in triangles) to these formats, my work was more involved with volumetric models (models with interior volume filled, represented by voxels or other polyhedra). 

## Goals

### Goal 1: Gain an Understanding of the Project and How it Will Benefit the Scientific Community

Although this goal may seem fairly general at first glance, I think it is a relevant to the type of work this term involved. It’s easy to the importance and influence in software products that are mainstream in the industry, but during this term all the work was in the research phase. And much of that work cutting edge, meaning there was nothing to build on. Because of this, I think it’s important to estimate how the research could affect the industry and if there is anyone doing similar work. 3D GIS is an emerging field in modern computing and this work could directly impact this industry, especially in the case of volumetric models. There has been much work done in the way of surface meshes and triangles as this is the most common and efficient (in speed and space) way to render 3D models. But one under researched area is in the representation of volumetric models, in our case we wanted to render models with different soil layers and rock types on the web, in modern formats such as GLTF.

### Goal 2: Understand all the Different Formats Required for This Type of Work

There were a wide variety of formats encountered during this work. VTK itself had a different format for each model type, ‘vtp’ for poly-meshes, ‘vts’ and ‘vtu’ for volumetric grids. Then there were more commonly used formats for viewing models such as GLTF, Collada, Wavefront Object, and more. And lastly there were the formats required to represent our models as a HLOD model-set such as Cesium 3D Tiles or ESRI I3S. To be able to work on this project, a good understanding of these formats is required. To do this we need to read through a lot of documentation, and this proved to quite challenging since the quality of documentation varied greatly between the formats. Various converters were also created in a range of languages, mostly C++ but also some JavaScript converters in NodeJS. Although I’ve spent four months working on these technologies, and have learned quite a great deal about them, there is still much more that can be learned of options and features, and much more experience would be required to really master them. 

### Goal 3: Improve Problem Solving Skills

This goal may also sound very obvious to any work term, but it is especially important here. The work done during this work term has been the most challenging so far. It also has been the most rewarding when concepts start to manifest in results. In the process of solving one problem many other problems may arise that need to be rectified, and because of this efficient and creative solutions were necessary. This really honed my skills in solving problems, and thinking about the solution in more than one aspect. For instance when converting massive models into 3D Tiles, I had to think about things like: How large should each tile be? What size should each model in the HLOD dataset be to produce an efficient tileset to render in the map viewers? How should the converter be written so it doesn’t take days to produce a single tileset? Many different things had to be considered when creating a solution for a problem and this term was the greatest learning experience I had to improve my problem solving skills. 

## Conclusion

This work term has been the best learning experience I’ve had so far, and I’ve learned the most from this experience. Compared to other work terms, where I was mostly working on routine tasks such as implementing features or writing documentation, this has been the most challenging and rewarding work that I have done. It has given me a first hand look on what the software research world looks like and how tech looks in the research and development phase before it gains momentum and support in the industry. 

## Acknowledgements

Big thank you to Boyan for giving me the opportunity, providing great feedback during our meetings, and asking tough questions to keep me on my toes. Also to Mike, for being a great mentor, helping me through issues, guiding me through concepts that I had never encountered before, providing a great internship experience during this crazy pandemic, and being a great friend to talk to. 












