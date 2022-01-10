We will discuss some of these questions in class if time permits.
Otherwise, you can consider them extra, not-for-credit practice questions that
will help with understanding course material and studying for the exam.

No need to report the answers to me --
this is just for practice and will not be graded.
I will not be releasing answers for them,
but I am happy to discuss them in office hours if you want to review any of
them.

Note: some questions are taken entirely or in part from your textbook.

# General Questions

1. Consider the following characteristic table:

A | X | Y | Xnext | Ynext
--- | --- | --- | --- | --- |
0 | 0 | 0 | 1 | 0
0 | 0 | 1 | 0 | 1
0 | 1 | 0 | 0 | 1
0 | 1 | 1 | 0 | 0
1 | 0 | 0 | 0 | 1
1 | 0 | 1 | 0 | 1
1 | 1 | 0 | 1 | 0
1 | 1 | 1 | 0 | 0

Draw a synchronous sequential circuit that has this characteristic table.
*Hint:* If you are not sure where to start,
pretend that `X` and `Y` have nothing to do with `Xnext` and `Ynext`.
That is, assume they are just inputs `B` and `C`.
Then, draw the corresponding combinational circuit.
From there, it is a small change to make the circuit synchronous sequential.

2. Consider a circuit corresponding to the table above.
Draw the timing diagram for the circuit in the following scenario.

* The initial inputs and state are `(0, 0, 0)`
* The value of `A` is held fixed at `0` for the first three clock ticks,
  then switches to `1`

3. Consider the following scenario.
A golfer will hit a good shot if it is sunny and there is no wind.
They will hit a bad shot any time there is wind.
If it is not sunny and there is no wind,
then the golfer will continue to play how they have been --
if their previous shot was bad,
their next shot will be bad,
and if their previous shot was good,
their next shot will be good.

Draw a characteristic table describing the golfer's behavior.

4. Draw a circuit corresponding to the situation above.

5. Choose some initial state and some values for the inputs and draw a timing
diagram for the golfer's behavior.
