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

# Practice Questions

These questions don't require thinking about things in a new way so much as
following instructions.
That does not mean that they are easy or unimportant,
but it does mean that they are not the best discussion questions.

We may do some of these as a warm-up and/or come back to them if we have time,
but we likely will not get through them all.
If you are not confident that you know how to solve these and we do not have
time to discuss them today,
please come see me in office hours so we can work through them together.

P1. Give the value of the following base-7 number in base 10:
143

P2. Give the hexadecimal equivalent of the following decimal number:
257

P3. Convert the following binary number to hex:
`1101101`

P4. What is `10010_2 / 2`?
You may want to verify your answer by converting to decimal,
but you should be able to solve the question without needing to convert.

P5. What range of numbers can be represented in 6 bits using
* unsigned binary numbers?
* two's complement binary numbers?

# General Questions

**Note:** In these activities, and *anywhere else in the course*,
if I mention signed binary numbers without specifying the format,
I am referring to two's complement numbers.

1. Base 16 (hex) numbers are useful because they are a shorthand way of writing
binary.
Two hex digits are the equivalent of one byte (8 bits).
What base could we use if we wanted to represent each byte with a single digit?
Why is that not common?

2. If an animal shelter is holding 18 stray dogs and wants to assign each of
them a unique numeric ID,
what is the fewest number of bits they would need to allocate to store an ID?

3. Consider 5 foods: apples, carrots, grapes, cookies, celery sticks.
Draw a circuit that determines whether a given food is a fruit.
This needs to occur in two steps:
* Choose a representation for the foods that a circuit will understand.
There is no single correct representation,
though some might be easier to work with.
* Draw the circuit. Writing a truth table first may be helpful.
Your circuit can output either True or False if an invalid input is given --
i.e., don't worry about invalid inputs for this question

4. Given a fixed size of 6 bits,
which binary system can represent more numbers:
unsigned or two's complement signed?
Explain.

5. Assume you have built an adder that computes the sum of two unsigned 16-bit
binary numbers.
How would you modify your adder to produce the sum of two signed 16-bit binary
numbers.

6. What is the decimal equivalent of the *signed* binary number `1101_2`?

7. Given your previous answer,
for each system,
provide an example of two binary numbers that result in overflow when added.

8. Consider the following operation: `1101_2 + 0111_2`.
Would the operation overflow using
* unsigned arithmetic?
* siged arithmetic?

9. Design a circuit that multiplies two one-bit numbers.
(We will not work with binary multiplication in this course,
except in powers of two.
This is just for circuit design practice.)

10. A 16-bit adder is still a combinational circuit because its outputs depend
only on its inputs.
How many rows would there be in the truth table for a 16-bit adder?
Don't forget about the carry in.

![example circuit](images/critical_path_1.jpg)

11. Assume all gates cause a delay of 10 nanoseconds.
What is the critical path through the circuit above?

12. Assume NOT gates cause a delay of just 3 nanoseconds,
but all other gates cause a delay of 10 nanoseconds.
Does that change the critical path through the circuit above?
Why or why not?

**Note:** There were not any Boolean algebra questions included here.
This is because they will be covered on the homework --
it does not mean you should ignore Boolean algebra.
