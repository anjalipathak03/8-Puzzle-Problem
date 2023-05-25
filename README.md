 # `8-puzzle problem using A* algorithm`
 
- WHAT IS 8-PUZZLE PROBLEM ?

Definition:
“It has set off a 3x3 board having 9 block spaces out of which 8 blocks having tiles bearing number from 1 to 8. One space is left blank. The tile adjacent to blank space can move into it. We have to arrange the tiles in a sequence for getting the goal state”.

Procedure:
The 8-puzzle problem belongs to the category of “sliding block puzzle” type of problem. The 8-puzzle i s a square tray in which eight square tiles are placed. The remaining ninth square is uncovered. Each tile in the tray has a number on it.

A tile that is adjacent to blank space can be slide into that space. The game consists of a starting position and a specified goal position. The goal is to transform the starting position into the goal position by sliding the tiles around.
The control mechanisms for an 8-puzzle solver must keep track of the order in which operations are performed, so that the operations can be undone one at a time if necessary. The objective of the puzzles is to find a sequence of tile movements that leads from a starting configuration to a goal configuration such as two situations given below.

Figure            (Starting State)                              (Goal State)

![image](https://github.com/03anjali/8-Puzzle-Problem/assets/91782986/afa0c5ec-66a2-41e4-82a6-e06659f7887c)


The state of 8-puzzle is the different permutation of tiles within the frame. The operations are the permissible moves up, down, left, right. Here at each step of the problem a function f(x) will be defined which is the combination of g(x) and h(x).

i.e. F(x)=g(x) + h (x)

Where

g (x): how many steps in the problem you have already done or the current state from the initial state.

h (x): Number of ways through which you can reach at the goal state from the current state or Or
h (x): is the heuristic estimator that compares the current state with the goal state note down how many states are displaced from the initial or the current state. After calculating the f value at each step finally take the smallest f (x) value at every step and choose that as the next current state to get the goal

We also know the eight puzzle problem by the name of N puzzle problem or sliding puzzle problem.

N-puzzle that consists of N tiles (N+1 titles with an empty tile) where N can be 8, 15, 24 and so on.
The 8-puzzle is a square board with 9 positions, filled by 8 numbered tiles and one gap. At any point, a tile adjacent to the gap can be moved into the gap, creating a new gap position. In other words the gap can be swapped with an adjacent (horizontally and vertically) tile. The objective in the game is to begin with an arbitrary configuration of tiles, and move them so as to get the numbered tiles arranged in ascending order either running around the perimeter of the board or ordered from left to right, with 1 in the top left-hand position.

- A* ALGORITHM

It is a searching algorithm that is used to find the shortest path between an initial and a final point.

It is a handy algorithm that is often used for map traversal to find the shortest path to be taken. A* was initially designed as a graph traversal problem, to help build a robot that can find its own course. It still remains a widely popular algorithm for graph traversal.

It searches for shorter paths first, thus making it an optimal and complete algorithm. An optimal algorithm will find the least cost outcome for a problem, while a complete algorithm finds all the possible outcomes of a problem.

Another aspect that makes A* so powerful is the use of weighted graphs in its implementation. A weighted graph uses numbers to represent the cost of taking each path or course of action. This means that the algorithms can take the path with the least cost, and find the best route in terms of distance and time.

![image](https://github.com/03anjali/8-Puzzle-Problem/assets/91782986/9c658011-34f2-468b-8cbe-8a90bf8b3349)

A major drawback of the algorithm is its space and time complexity. It takes a large amount of space to store all possible paths and a lot of time to find them.
