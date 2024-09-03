**PART 1: FAIRIES, HEURISTICS, AND A***

Problem Statement:

Five fairies with unique symbols want to arrange themselves in ascending order quickly by swapping with their neighbors. Modify the BFS-based solution to an A* algorithm with a priority queue and an admissible heuristic. Ensure all cases in "fairies.txt" can be solved within 10 seconds.

Initial State: 

The initial state represents the starting configuration of the fairies. In this state, the symbols on the fairies are arranged in a random order. 
EXAMPLE: FROM [1, 3, 4, 2, 5]

Goal State:

The goal state represents the desired configuration of the fairies. In this state, the symbols on the fairies are arranged in ascending order, starting from 1 and ending at N (where N is the number of fairies).
EXAMPLE: TO [1, 2, 3, 4, 5]

Successor function: 

The successor function serves the purpose of generating all possible successor states from the current state in the fairy rearrangement problem. In this problem, each fairy can gracefully switch places with one of her neighboring companions in a single step. Therefore, the successor function generates all valid states that can be reached by swapping neighboring fairies, one pair at a time.

Heuristic Function:

The heuristic function serves the purpose of providing an estimate of the cost, specifically the number of steps, required to reach the goal state from the current state in the fairy rearrangement problem.

The Algorithm:

The A* search algorithm is employed to find the optimal sequence of moves that transforms the initial state of the fairies into the goal state. The A* search algorithm, with the provided heuristic function and successor function, significantly improves the performance compared to the original BFS-based solution.
