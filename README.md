#### Mouse with scroll wheel required. 
Left click - Start position  
Right click - End position  
Middle scroll wheel click - Draw Wall  
Space - Begin search  

# Dijkstra's Algorithm

Both Dijkstra's and A* algorithms work by finding the shorted path between two points. 
Dijsktra's essentially "floods" the entire grid beginning from a starting source location,
numbering every node with the distance traveled. Upon reaching the destination node, the algorithm decrements
backwards to the starting position (0), determining the minimal path.

![Alt text](/Screenshots/dij_pathfinding.png?raw=true "Cover")
![Alt text](/Screenshots/dij_path_found.png?raw=true "Cover")

# A-Star

A*'s pathfinding implemention begins similarly: all visited nodes record the distance traveled
out from the starting node. Unique to A*, nodes <i> also </i> remember the relative distance from the current position to the destination node (a simple Pythagorean calculation).
In this way, the algorithm more effectively 'predicts' which visited
nodes are more likely to be a shorter distance to the finish, and continues from them before moving to nodes
with lower calculated 'weight.'

![Alt text](/Screenshots/A_star.png?raw=true "Cover")
![Alt text](/Screenshots/A_star_found.png?raw=true "Cover")
