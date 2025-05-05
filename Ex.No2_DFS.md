# Ex.No: 2  Implementation of Depth First Search
### DATE:  11/03/2025                                                            
### REGISTER NUMBER : 212222220056
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:
```
graph = {
    '5': ['3', '7'],
    '3': ['2', '4'],
    '7': ['8'],
    '2': [],
    '4': ['8'],
    '8': []
}

visited = set()  # Set to keep track of visited nodes.

def dfs(visited, graph, node):  # Function for DFS
    if node not in visited:
        print(node, end=" ")  # Print the node
        visited.add(node)
        for neighbour in graph[node]:
            dfs(visited, graph, neighbour)

# Driver Code
print("Following is the Depth-First Search:")
dfs(visited, graph, '5')

```











### Output:



![ex2ai](https://github.com/user-attachments/assets/f24066ee-9da2-4a64-99e2-e09863779569)


### Result:
Thus the depth first search order was found sucessfully.
