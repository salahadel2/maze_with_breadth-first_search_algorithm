# maze_with_breadth-first_search_algorithm
maze-solving algorithm using breadth-first search
## breadth-first search is a search algorithm that always expands the shallowest node in the frontier before moving deeper.
### frontier :- implemented using a queue data structure, **queue** is a first-in first-out data type.
### breadth-first search algorithm steps:-
• Start with a frontier that contains the initial state. 
• Start with an empty explored set. 
• Repeat: 
• If the frontier is empty, then no solution. 
• Remove a node from the frontier. 
• If node contains goal state, return the solution. 
• Add the node to the explored set. 
• Expand node, add resulting nodes to the frontier if they 
aren't already in the frontier or the explored set.

### Breadth-first search algorithm Pseudocode:-

BreadthFirstSearch(start, goal):
    Create an empty queue frontier
    Enqueue the start node onto the frontier
    
    Create an empty set explored
    
    while frontier is not empty:
        node = Dequeue the front node from the frontier
        
        if node is the goal:
            return node  // Solution found
        
        Add node to explored set
        
        for each neighbor in neighbors of node:
            if neighbor is not in explored and not in frontier:
                Enqueue neighbor onto the frontier
                
    return None  // No solution found

