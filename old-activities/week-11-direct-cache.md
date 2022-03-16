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

8. The following function does not preserve registers correctly.
   Modify it so that it does.

   ```
   fun:
        addi $s0, $0, 8
        addi $t1, $0, 4

        slt $t4, $a0, $s0
        slt $t5, $t1, $a0
        and $v0, $t4, $t5

        jr $ra
   ```

9. A compiler takes high-level code and converts it to assembly code.
   Given how close assembly code is to machine code,
   what useful purpose(s) does the assembler serve?
   (You have likely never called an assembler directly --
   your compiler calls it for you.)

1. What is a `syscall` in MIPS?
   Give two examples of things you can do with a `syscall`.

2. The base address of an array is stored in `$t0`.
   How does the process of accessing the second element array change,
   if at all,
   depending on whether the array is on the stack, the heap, or in global
   memory?

3. The code below does not do what the comments suggest.
   How would you fix the code to match the comments?

   ```
   .data

        x: .word 40
        s: .asciiz "abc123"

   .text
        # x += 5
        addi $t0, x, 5
        sw $t0, x

        # grab second character of string ('b')
        la $t1, s
        addi $t1, $t1, 4
        lw $t2, 0($t1)
   ```

4. Describe in your own words what a cache is.
   <!-- Small, fast memory where we hold data we expect we will need in the
   near future. -->

5. How, if at all, does the use of a cache change
    * the results of a program?
    * the performance of a program?

6. What is temporal locality?
   Give an example of temporal locality in your daily life.

7. What is spatial locality?
   Give an example of spatial locality in your daily life.

<!--
1. Looking at the memory hierarchy,
   (cheap) memory that we have a lot of is always slower than (expensive)
   memory that we do not have a lot of.
   Why are there no fast, cheap, and large options?

   Answer: because if something were both faster *and* cheaper,
   we would replace the other kind entirely.
   Put another way, our memory *is* big, fast, and cheap compared to older
   technologies.
-->

8. Start working on the
   [direct-mapped cache handout](/misc/direct-cache-handout.pdf).
