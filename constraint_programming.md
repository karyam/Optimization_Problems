## Constraint programming
   - **computational paradigm** which
     - uses constraints to **reduce the search space** for each variable; remove values that cannot appear in any solution
     - **makes a choice** when no more deducions can be performed
     - when a choice is wrong, **backtrack**
   - is a complete method, not heuristic
   - given enough time finds the optimal solution for an OMP problem
   - focus on feasibility
   - uses **Branch and pruning**
     - **branching**: decompse the problem into subproblems and solve the subproblems
     - **pruning**: 