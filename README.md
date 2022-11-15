# Artificial Intelligence Foundations and Applications (AI61005) IIT Kharagpur - Term Assignment

## Multi Agent Pathfinding Problem using Conflict Based Search (CBS) and its applications in Agriculture

### Introduction

Multi-agent pathfinding algorithm is responsible for finding the paths for multiple agents from their current locations to their target locations without colliding with each other, while at the same time optimizing a global cost function, such as the sum of the path lengths of all agents. 


The problem is formulated by giving the input for the coordinates of the source and the destinations, with the obstacles given as the points that cannot be accessed by the agents. We assume the workhouse as a matrix with the coordinates representing the desired location.

The path of the agents in which the cell are in normal state, only one robot can exist in that cell. We develop an algorithm to get the tasks done in the minimum time possible. The methodology is discussed in further detail ![here](https://github.com/jainaviral898/mapp-cbs-aifa/blob/main/AIFA%20Term%20Assignment.pdf).

![image](https://user-images.githubusercontent.com/50842568/140016269-78703773-f00a-44aa-b2d2-ec59d632679a.png)

### Conflict-Based Search Algorithm
CBS is a two-level algorithm that converts the problem into the single ‘joint agent’ model. At the high level, a search is performed on a Conflict Tree (CT) which is a tree based on conflicts between individual agents. Each node in the CT represents a set of constraints on the motion of the agents. At the low level, fast single-agent searches are performed to satisfy the constraints imposed by the high-level CT node. In many cases, this two-level formulation enables CBS to examine fewer states than A* while still maintaining optimality.
### Input Format

Use the "input.yaml" file to give the inputs, fill in the stops made by the robots.
The obstacles are to be included in the given format. 

### References

1. MULTI-AGENT PATH PLANNING OF ROBOTIC SWARMS IN AGRICULTURAL FIELDS (N. Botteghi, A. Kamilaris,  L. Sinai, B. Sirmacek)
2. Improved Heuristics for Multi-Agent Path Finding with Conflict-Based Search Jiaoyang Li , Ariel Felner, Eli Boyarski , Hang Ma and Sven Koenig.


### Team Details

Aviral Jain - 18AG3AI08

Sumit Kumar - 18AG3AI10
