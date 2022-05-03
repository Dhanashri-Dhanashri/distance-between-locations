# distance-between-locations
**Code to develop a scalable data structure where one can add a new city and corresponding distance from all the existing cities in the system.**
Example : 
Enter the root city: Noida
Enter a new city: Delhi
Enter the distance from Noida: 50

Enter a new city: Mumbai
Enter the distance from Noida: 1400
Enter the distance from Delhi: 1350

Enter a new city: Bengaluru
Enter the distance from Noida: 2150
Enter the distance from Delhi: 2100
Enter the distance from Mumbai: 1000

**NOTE: UI part is skipped, could be developed based on user interest**
The data strcuture developed is a graph using Python Programming language.

In the code we create two classes, Graph which holds list of vertices and Vertex which represents each vertex in the graph.

The Graph class contains a dictionary that maps vertex names to vertex objects, and we can see the output by the __str__() method of Vertex class:
g.vert_dict[Noida]=Noida adjacent: ['Delhi', 'Mumbai', 'Bengaluru']
Graph also provides methods for 
- To add vertices to a graph and connecting one vertex to another. 
- To return the names of all of the vertices in the graph.
- Iterator is used to make it easy to iterate over all the vertex objects in a particular graph.

The Vertex class uses a dictionary to keep track of the vertices to which it is connected, and the weight of each edge. The Vertex constructor initializes the id, which is usually a string, and the adjacent dictionary. 
Vertex provides methods like :
- The add_neighbor() method is used add a connection from this vertex to another. 
- The get_connections() method returns all of the vertices in the adjacency list. 
- The get_weight() method returns the weight of the edge from this vertex to the vertex passed as a parameter.

In main(), we created vertices labelled with names of cities like Noida, Delhi, Mumbai, Bengaluru. This can vary based on the question.
Then we displayed the vertex dictionary. Notice that for each key, we have created an instance of a Vertex. Next, we add the edges that connect the vertices together. Finally, a nested loop verifies that each edge in the graph is properly stored.

![image](https://user-images.githubusercontent.com/55523316/166448829-35ebcb20-1d9d-47de-86b9-b31a40c8e4a9.png)
