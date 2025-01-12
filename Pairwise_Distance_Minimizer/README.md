# Pairwise Distance Minimizer Theory Based Project

This was the capstone project completed during UC Berkeley's algorithms course. 

## Premise
Formally, let G= (V,E) be a positive weighted, connected, undirected graph.  We would like to find a subgraph T ofG such that:
1. Every vertexv ∈ Vis either in T or adjacent to a vertex in T
2. T is a tree
3. The average pairwise distance between all vertices in T is minimized.



## Approach
We used a combined approach of leaf (node) prunning and Prim's algorithm. 
Please see the reflection for more details on the technical approach.

## Installation & Requirements
The files needed for the project are below.

Required Files:
- `parse.py`: functions to read/write inputs and outputs
- `solver.py`: where you should be writing your code to solve inputs
- `utils.py`: contains functions to compute cost and validate NetworkX graphs
- 'submission'.json: Our submission
- 'team.txt': Txt file containing our team name and SIDS
- 'prepare_submission.py': Staff written python file to prepare out submission
- 'submission' as an empty directory to hold our outputs (you must make this)
- 'inputs' as an directory to hold your inputs (you must make this)


The requirements are below:
-If using pip to download, run python3 -m pip install networkx
- Sys, os, operator, random, and copy

## Running the Program
- Simply run ##python3 solver.py## to generate outputs. Note that print statements may occur. You may comment them out
for a cleaner view.
- Some outputs *may* (namely medium-111.in) be invalid or blank. We manually added 0 to those files.
- Because the base case depends on randomness to some degree, you may get a recursion depth error, though
precautions have been added to avoid this. Note that no recursion depth errors occured even without the added
protection when running on instructional machines. We recommend you run this on the hive.
- If you are still getting a recursion depth error, don't worry. We have designed an advanced recursion depth prevention system, simply
uncomment lines 53 and 54.
