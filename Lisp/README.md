# LMC Project: Lisp

Group components:

- Davide Cologni
- Davide Cestari
- Giorgio Bertolotti

The lmc.lisp file refers to an implementation of an LMC (Little Man Computer) simulator written in CommonLisp language.

The main functions required in the assignment text are the following:

- one-instruction State -> NewState
	> Function which takes the instruction from the memory in *State*, executes it and returns the next state *NewState*.

- execution-loop State -> Out
	> Function which executes in loop *one-instruction* until it reaches the halted state. It returns *Out*, which is the output queue of the final state.

- lmc-load FileName -> Mem
	> Function which reads an *assembly* file and returns the initialized memory.

- lmc-run FileName Input -> Out
	> Reads the file *FileName* using *lmc-load* and executes it using *execution-loop*.