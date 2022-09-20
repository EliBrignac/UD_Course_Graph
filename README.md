# UD_Course_Graph

### Graph of courses that CISC 108 is a prereq for and beyond (CISC 108 = Introduction to Computer Science I)
![CISC 108](https://user-images.githubusercontent.com/94129362/191188459-e2d990e8-bccc-4d53-9139-e4cb78d9c9c9.png)

## Introduction:
When I was deciding on what courses to take at UD I ran into a problem. I was trying to choose between 2 courses, and wanted to know what doors each one would open up for me. However, the courses listed on the course catalog only show the prereqisites, not the courses that come after. So I decided to make this jupyter notebook that builds a graph of all the courses that come after the course of interest (the course of interest is a prereq for these "after_coureses")

### Partially Completed
For my general purposes of math and computer science, this project is basically done, but I may continue to improve it as I see this as a potentially useful tool for all UD students. Some simple improvements I have in mind are...
- Better Webscraping method to get data faster. In particular, finding a way to parse the info directly from the first link rather than going to a referenced link to get the info.
- Better Graph functions such as num of edges, neighboring nodes, printing the first 2 layers, etc. This is easy to implement with pydot
- Mass saving the images of the graphs.



