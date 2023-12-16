# Algorithms and Data Structures Phase-3: Graph Algorithms

This repository is part of a comprehensive educational series for an Algorithms and Data Structures class, focusing on graph algorithms. The project applies graph algorithms to simulate connectivity between health centers and find optimal paths for logistics or emergency services.

## About The Project

The project includes an implementation of a graph, where vertices represent health centers and edges represent the connectivity and distance between them. It demonstrates the use of classic graph algorithms like Dijkstra, Bellman-Ford, and Floyd-Warshall to find the shortest paths and connectivity in the network.

### Features

- Graph representation of health centers.
- Implementation of Dijkstra's algorithm for shortest path finding.
- Implementation of Bellman-Ford algorithm to accommodate negative weights and detect negative cycles.
- Implementation of Floyd-Warshall algorithm for all-pair shortest path computation.

## Usage

The `Map` class can be used to create a map of health centers and their connections. You can then use the provided algorithms to find shortest paths:

```
from fase3 import Map, HealthCenter

# Create a map
health_map = Map()

# Add health centers
health_center_A = HealthCenter('A')
health_center_B = HealthCenter('B')
health_map.addHealthCenter(health_center_A)
health_map.addHealthCenter(health_center_B)

# Connect health centers
health_map.addConnection(health_center_A, health_center_B, distance=10)

# Find shortest path
path, distance = health_map.minimumPath(health_center_A, health_center_B)
print("Shortest path:", path)
print("Distance:", distance)
```

## Contact

Rosa Reyes: [LinkedIn](https://www.linkedin.com/in/rosaareyesc/)
