# UD_Course_Graph

### Graph of courses that CISC 108 is a prereq for and beyond (CISC 108 = Introduction to Computer Science I)
![CISC 108](https://user-images.githubusercontent.com/94129362/191188459-e2d990e8-bccc-4d53-9139-e4cb78d9c9c9.png)

## Introduction:
When I was deciding on what courses to take at UD I ran into a problem. I was trying to choose between 2 courses, and wanted to know what doors each one would open up for me. However, the courses listed on the course catalog only show the prereqisites, not the courses that come after. So I decided to make this jupyter notebook that builds a graph of all the courses that come after the course of interest (the course of interest is a prereq for these "after_coureses")


## How to use:
- Run all of the cells top to bottom. This takes ~60 seconds (Don't worry about the stuff being printed that is for debugging purposes 😎)
- Once output stops, add a new cell and use the function ```get_graph_image("course name here")``` to output an image of the course of your choice
  - Example: ```get_graph_image("CISC 108")```
  - Example: ```get_graph_image("MATH 241")```
- To print every course, call the function ```get_all_graph_images()``` 

### Partially Completed
For my general purposes of helping me choose math and computer science courses, this project is basically done, but I may continue to improve it as I originally saw this as a potentially useful tool for all UD students. Some simple improvements I have in mind are...

- **Getting information from all course types, not just MATH and CISC**
  - This currently only webscrapes the data for MATH and CISC courses
- **Better Webscraping method to get data faster.** 
  - In particular, finding a way to parse the info directly from the first link rather than going to a referenced link to get the info. This could improve the speed ~40x-100x and really allow for scalability, however I am not yet sure if its possible to do.
- **More Graph functions** 
  - Functions for the number of edges, neighboring nodes, only printing the first 2 layers, etc. This is easy to implement with pydot and my knowledge of graphs.
- **Ability to save the images** 
  - Save images of graphs directly to your computer. This also shouldn't be that difficult as Pillow (PIL) is a great tool I've used in the past to acheive this 
- **Option to output more information in each node**
  - Give the option to output the course description, title, prereqs, etc, within each displayed node on the graph
- **Option to output prereqs of different course types**
  - Example: MATH 210 is a prereq for CISC 320, but they are of different course types so there will not be an edge drawn between the two.
- **Potentially have this recognized by UD and hope they implement someway in their course catalog service**



