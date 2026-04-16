# -COMP-2090SEF-group-project-task-2
Our purpose is to learn about Trie-Data-Structure and Dijkstra-s-Algorithm

#User Guide – Trie Data Structure (Python)
1. Prerequisites
Python Version: Ensure you have Python 3.8 or above installed.
Environment: Works on Windows, macOS, or Linux.
Editor/IDE: You can use any text editor (VS Code, PyCharm, IDLE, etc.) or run directly from the terminal/command prompt.
Check your Python version:
python --version
2. Download the Code
Save the provided Trie implementation into a file named trie.py.
Example structure:
project_folder/
    trie.py
3. Running the Code
Open a terminal in the project folder and run:
bash
python trie.py
This will execute the example usage included in the if __name__ == "__main__": block.
4. Expected Output
When you run the code, you should see:
程式碼
True
True
False
True
True
False
Explanation:
search("apple") → True (word exists)
search("app") → True (word exists)
search("appl") → False (not a complete word)
starts_with("ap") → True (prefix exists)
starts_with("ba") → True (prefix exists)
starts_with("cat") → False (prefix not found)
5. How to Use in Your Own Programs
You can import the Trie class into other Python files:
python
from trie import Trie

trie = Trie()
trie.insert("hello")
print(trie.search("hello"))       # True
print(trie.starts_with("he"))     # True
6. Extending the Code
Add an autocomplete function to return all words starting with a given prefix.
Store words from a dictionary file for spell-checking.
Integrate into larger projects (e.g., search engines, text editors).   

#User Guide – Dijkstra’s Algorithm
1. Prerequisites
Python Version: Python 3.8 or above.
Environment: Works on Windows, macOS, or Linux.
Editor/IDE: Any text editor or IDE (VS Code, PyCharm, IDLE).
Check Python version:
bash
python --version
2. Download the Code
Save the above code into a file named dijkstra.py.
Project structure:
程式碼
project_folder/
    dijkstra.py
3. Running the Code
Open a terminal in the project folder and run:
bash
python dijkstra.py
4. Expected Output
You should see:
程式碼
Shortest paths from A:
  A: 0
  B: 4
  C: 2
  D: 9
  E: 5
  F: 20
Explanation:
Distance from A to B is 4.
Distance from A to C is 2.
Shortest path to D goes through C -> E -> D with total cost 9.
Path to F is longer, total cost 20.
5. How to Use in Your Own Programs
You can import the Graph class into other Python files:
python
from dijkstra import Graph

g = Graph()
g.add_edge("X", "Y", 7)
g.add_edge("X", "Z", 3)

print(g.dijkstra("X"))
6. Extensions
Modify to handle undirected graphs by adding edges in both directions.
Track actual paths (not just distances) by storing predecessors.
Integrate into applications like GPS navigation, network routing, or optimization problems.

