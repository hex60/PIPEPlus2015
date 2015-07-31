# PIPEPlus2015
A High Level Petri Net Modeling and Analysis Environment, which is built upon
the PIPE platform for Low Level Petri nets. This environment includes a graphical 
editor for creating high level Petri nets (predicate transition nets where arcs
are labeled with variable expressions and transitions contain logic formulas). 
Two basic token data types, integer and string, are supported. Structured data types
such as Cartesian product (tuples) and power set (only one level) can be built on the
basic data types. These data types are used to define the token types of places.

Three analysis approaches are currently supported:
(1) Simulation - firing transitions stepwisely (automatically firing all enabled transition can easily done
by commenting out a break statement;
(2) Model checking - a HLPN model is automatically translated into a Promela program together with a given temporal logic
formula, which are checked by SPIN model checker;
(3) Bounded model checking - a HLPN model is automatically translated into SMT-lib form to be solved using Z3 SMT solver.

This environment was mainly developed by my former Ph.D. students Dr. Su Liu with contributions from Dr. Reng Zeng starting
around 2010. There stiil exist many bugs, which are constantly fixed.
 
