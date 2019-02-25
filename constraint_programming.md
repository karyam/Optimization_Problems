## Constraint programming
   - **computational paradigm** which
     - uses constraints to **reduce the search space** for each variable; remove values that cannot appear in any solution
     - **makes a choice** when no more deducions can be performed
     - when a choice is wrong, **backtrack**
   - is a complete method, not heuristic
   - given enough time finds the optimal solution for an OMP problem
   - focus on feasibility
   - uses **Branch and pruning**
     - **branching**: decompse the problem into subproblems and solve the subproblems (try all possible values for a variable until a solution is found or it can be proven than no solution exists)
     - **pruning**: use constraints to remove, from the variable domains, values that cannot belong to any solution
     <pre><code> propagate(){
         repeat
           select a constraint c;
           if c is infeasible given the domain store then
             return failure;
           else
             apply the pruning algorithm associated with c;
          untill no constrint can remove any value from the domain of its variables
         return success;
       }
     </code></pre>
