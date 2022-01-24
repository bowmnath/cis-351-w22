In your groups, answer the following questions.
No need to report the answers to me --
this is just for practice.
We may not get through all of the questions every week.
You may want to take notes during the discussion,
because these questions will be helpful in reviewing for exams.

I will be dropping in and out of rooms to facilitate to the discussions and in
case you have any questions.
Think of it like me walking around the classroom and listening to different
groups.
Again, this isn't meant to be for a grade,
so don't be concerned about giving a wrong answer even if I am in the room.
You can also flag me down in Zoom if you have a question even if I'm not in the
room
(I think the button in Zoom looks like a question mark).

Note: some questions are taken entirely or in part from your textbook.

# General Questions

1. Consider 3 sports: javelin, soccer, and baseball.
Draw a circuit that determines whether a given sport requires a ball.
This needs to occur in two steps:
* Choose a representation for the foods that a circuit will understand.
There is no single correct representation,
though some might be easier to work with.
* Draw the circuit. Writing a truth table first may be helpful.
Your circuit can output either True or False if an invalid input is given --
i.e., don't worry about invalid inputs for this question

![example circuit](images/critical_path_1.jpg)

2. Assume all gates cause a delay of 10 nanoseconds.
What is the critical path through the circuit above?

3. Assume NOT gates cause a delay of just 3 nanoseconds,
but all other gates cause a delay of 10 nanoseconds.
Does that change the critical path through the circuit above?
Why or why not?

When answering the next few questions,
consider what you learned about **critical paths**.
This is an important concept that will show up throughout your career and daily
life if you know to look for it.

4. Building a house has the following (completely made-up) requirements:
* Pouring the foundation. Time cost: 2 weeks
* Building the framing, which requires a foundation. Time cost: 4 weeks
* Adding sideing, which requires a frame. Time cost: 1 week
* Adding a roof, which requires a frame. Time cost: 2 weeks
* Adding doors, which requires sideing. Time cost: 0.5 week
* Adding windows, which requires sideing. Time cost: 0.75 week
* Interior work, which requires a roof. Time cost: 4 weeks

How long does it take to build a house?

5. In the example above,
if the roof is delayed by one week,
how does this change the time for the overall project?

6. Are there any steps that can be delayed *without* causing the production of
the house to be delayed?
If so, list all of them.
If not, explain why not.

7. You are working on a group project and decide to split up tasks among
group members.
However, you have a group member who you are pretty sure will not finish
whatever tasks they are assigned in a timely manner.
How can the concept of a critical path help you in this situation?

<!-- can't do anything below here today -->

8. Consider the following mux and inputs.
Note that the selector input is given in binary (hence the `B`).
What is the output?
How could you change the selector to get a different output?

![simple mux](images/simple_mux_1.jpg)

<!-- ascii mux
```
    01
    |
   |-
 1-| \
 0-| |
 0-| |---
 0-| /
   |-

```
-->

9. Consider a circuit with two inputs: `Num` (two bits) and `DoNot` (one bit).
If `DoNot` is 0, the circuit outputs `Num`.
Otherwise, the circuit outputs the bitwise NOT of `Num`.
Create the circuit described using only muxes and NOT gates.

10. If `Num` were considered as a two's complement binary number,
would the circuit above compute `-Num` when `DoNot` was `1`?
Why or why not?

11. Represent the Boolean expression
`A + (B xor C)`
using only a multiplexor.

12. Consider representing the Boolean expression
`(A + B)*(C + ~A) + D + (E*F) + (F xor G)`
using a multiplexor.
    * how many selector inputs would be required?
    * how many data inputs?

13. Why might representing the expression above using a multiplexor be a bad
idea?
How does this relate to truth tables?

14. Your lab partner wants to speed up your 16-bit adder using the following
idea:
   * use two 16-bit ripple-carry adders,
   one with a carry-in of 1 and the other with a carry-in of 0
   * attach the outputs to multiplexors and use the actual carry in as the
   selector for the muxes
How would you explain to them that this is a bad idea?
How could the idea be improved?

15. Given `G3:2`, `G_1:0`, `P_3:2`, `P_1:0`, and a carry-in `C_in`,
give a Boolean expression to determine `C_3`.
That is, if you know the generate and propogate logic for 2-bit blocks,
how can you determine the carry-out for the combined 4-bit block?
(Hint: The expression should look familiar.)
