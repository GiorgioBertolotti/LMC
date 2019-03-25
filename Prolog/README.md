# LMC Project: Prolog

Group components:

- Davide Cologni
- Davide Cestari
- Giorgio Bertolotti

The lmc.pl file refers to an implementation of an LMC (Little Man Computer) simulator written in Prolog language.

The main predicates required in the assignment text are the following:

- one_instruction(State, NewState)
	> Predicate which takes the next instruction from *State*, executes it and generates the next state *NewState*.

- execution_loop(State, Out)
	> Predicate which executes in loop the *one_instruction* predicate until it reaches the *halted_state*. *Out* is the output queue of the final state.

- lmc_load(FileName, Mem)
	> Predicate which reads an *assembly* file and initializes the memory.

- lmc_run(FileName, Inp, Out)
	> It sets the input queue of the LMC as *Inp* and generates *Out*, which is the result of the invocation of *execution_loop* predicate.