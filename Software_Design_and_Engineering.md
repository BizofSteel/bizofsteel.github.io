# Software Design and Engineering 

## The Artifact
For our _CS499 Computer Science Capstone_ course we were asked to select artifacts from previous experience for the purpose of expanding them in complexity to showcase our proficiency in the categories of Software Engineering and Design, Algorithms and Data structures, and Databases.  In this section I will be presenting my proficiency in Software Engineering and Design by expanding the complexity of an artifact from my CS 330: Computational Graphics and Visualization course.   The artifact itself is a model of a Listerine bottle that includes the use of different textures, lighting techniques, and rendering which was coded in C++ using OpenGL.

## Inclusion of Artifact in ePortfolio
I have chosen to include this artifact in my ePortfolio because the coding architecture of working with OpenGL and computational graphics is complex and showcases my understanding designing such a product.  To expand an artifact of this sort, one must have the ability to plan, design and plot vertices in 3D space, and engineer indices from those vertex points.  One must also understand how to work with OpenGL which includes being proficient with memory allocation, Buffers (specifically Vertex Buffer Object and Vertex Array Object), and software engineering to successfully render an image.  I chose to increase the complexity of this artifact because at the time when I took the course, I did not get a chance to really tap into the power of OpenGL.  I spent too much time learning the basics of this software.  Interestingly, while going through the course I learned how to implement more complexities like using multiple containers for memory management and different buffering techniques to get better results.  To improve my artifact, I did just this.  I designed and plotted new vertices to decrease pixilation through the curves of the bottle, deployed new Vertex Array Object to handle the increase in memory use, and consolidated software through strategic planning.

## Process of Enhancing Artifact
To create this artifact, I had to start with a basic design of the profile of the Bottle.  

![Figure 1](https://bizofsteel.github.io/Artifact%201%20-%20Fig%201.png) 

As Seen in Figure 1, I created a basic sketch to determine the different cross sections that would be used as my vertices plane.  Each horizonal line in this figure represents one of these planes (Appendix A).  Next, I plotted vertex locations on different cross sections for the purpose of creating index connections from plane to plane and create rendering triangles (surfaces).   Once my points were created, I deployed my Vertex Array Objects to render the object.   As you can see in this figure, the original design used two arrays, one for the Cap, and another for the main body of the bottle and one container each, respectively. 

These vertices were kept in containers that quickly ran out of memory and did not allow me to render the object.  To fix this problem, I simply decreased the number of indices and vertices deployed which pixelated my object.  

![Figure 2](https://bizofsteel.github.io/Artifact%201%20-%20Fig%202.png) 

As seen in Figure 2 shown in polygon mode, I was only able to achieve 36 triangles per revolution.  The purpose of the artifact was not to create high resolution renderings but to render successfully.  And while I met the requirements, I was left dissatisfied with the level of resolution of my object.  The enhancements that I now showcase herein shows my growth in engineering and executing work arounds to the container memory limitation, specifically those I was challenged with on my first time around. 
 
To enhance the artifact, I began with the re-plotting of the vertex planes.   

![Figure 3](https://bizofsteel.github.io/Artifact%201%20-%20Fig%203.png) 

Figure 3 shows the original cross-section (top) with plotted indices.  Notice that the new cross-section (bottom) has doubled the number of indices that will be used.  To handle the new memory requirements, the new data would have to be strategically distributed between different containers and efficient memory allocation. To enhance this capability, I increased the number of Vertex Array Objects from the original two (Figure 1) to a total of five as shown on Figure 4. 

![Figure 4](https://bizofsteel.github.io/Artifact%201%20-%20Fig%204.png) 

The new architecture is not only more efficient but also successful in deploying and rendering a total of 72 triangle per revolution which not only increases resolution but also helps with buffering.  The enhancement also consolidates an index call out as I have been able to consolidate “like” features into one container.   Specifically, the feature created by the TOP and BOT VAO’s are the same so the “bottleBumpIndices” is one container called upon respectively as shown on Figure 5.  This approach allows for ease of scaling, repeatability and increases efficiency in maintenance and sustainability of the code.



```markdown
**Computational Graphics and Visualization.**   
The artifact in this Section is a model of a Listerine bottle that includes the use of different textures, lighting techniques, and rendering

```




**Bismark J. Aldana ePorfolio Links**<br>
* [ePortfolio Homepage](https://bizofsteel.github.io)<br>
* [Refinement Plan & Code Review](https://bizofsteel.github.io/Code_Review.html)<br>
* [Software Design and Engineering - Enhancement One](https://bizofsteel.github.io/Software_Design_and_Engineering.html)<br>
* [Algorithms and Data Structures - Enhancement Two](https://bizofsteel.github.io/Algorithms_and_Data_Structure.html)<br>
* [Databases - Enhancement Three](https://bizofsteel.github.io/Databases.html)
