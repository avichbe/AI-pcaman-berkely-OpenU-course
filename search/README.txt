author: Avichay Ben Lulu 301088670
mmn:11

1.i use the hint and create function that made general-search - named graphSearch(problem, structure)-
each node contain - state,action,cost.
then using this graphSearch and util to search the problem with util.Stack().
DFS it's not the "cheapest" route because this is the BFS job.
DFS only guarantee to applicable route not the cheapest.
2. just change the structure to be queue. In this mode we will get the BFS which
Is the optimal route to the destination.
3. I change the structure to be priority queue – with each node get the prioritize by cost- this create the UCS algo.
4. I remain with the priority queue but change the lambda func that define cost.
Now change it to price + the value returned by heuristic func in state as parameter.
This gave us the Astar  algo.
In the open maze:
Astar manhatanHeuristic is the best with cost of 54 and 535 expanded nodes.
Astar nullHuer/BFS/UCS is the same  cost of 54 and 682 expanded nodes.
 DFS is the worst cost of 298.
We can see that manhatan heuristic is improved the performance of the ASTAR algo.
5.  I represent state as a tuple of (positions, corners) then moving corner by corner.
6. I implement the heuristic as Manhattan distance from the closest corner there for the algorithm, will prefer the closer route to the corner. 
7.  I choose to implement my heuristic as the distance to the farthermost food, provided by mazeDistance.   
8. I choose to use BFS in this Q. the cost is 350 as it asked.
