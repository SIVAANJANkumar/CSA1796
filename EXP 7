from collections import defaultdict, deque

class Graph:
    def __init__(self):
        self.graph = defaultdict(list)

    def add_edge(self, u, v):
        self.graph[u].append(v)

    def bfs(self, start_node):
        visited = set()
        queue = deque([start_node])

        while queue:
            current_node = queue.popleft()
            if current_node not in visited:
                print(current_node, end=" ")
                visited.add(current_node)
                queue.extend(node for node in self.graph[current_node] if node not in visited)

# Create a graph
g = Graph()
g.add_edge(0, 1)
g.add_edge(0, 2)
g.add_edge(1, 2)
g.add_edge(2, 0)
g.add_edge(2, 3)
g.add_edge(3, 3)

print("Breadth-First Traversal (starting from node 2):")
g.bfs(2)
