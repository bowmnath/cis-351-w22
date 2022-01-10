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

# Review

1. If you did not have time to get to it last week,
   at some point be sure that you understand the
   [assembly and memory handout](/misc/assembly-and-memory.pdf).

# General Questions

1. Consider the MIPS microarchitecture from your textbook.

   ![mips microarchitecture](images/mips-full-microarchitecture.png)

   What is the value of `MemtoReg` for each of the following instructions?
   Write an `X` if the value does not matter.
   * `lw`
   * `add`
   * `addi`
   * `bne`

2. The instructions above have the following opcodes:
   * `lw` -- `100011`
   * `add` -- `000000`
   * `addi` -- `001000`
   * `bne` -- `000101`

   Assuming those were the only instructions implemented,
   give an example of how the control logic for `MemtoReg` could look.
   Assume that any `X` above is treated as a `0`
   (though this is not necessarily the case in a real circuit.)

For the next few questions,
consider the array `[7, 99, 14, 12]` with base address `0x10004000`
as pictured below.

```
addr       | data
---        | ---
0x10004014 |   X
0x10004010 |   X
0x1000400c |  12
0x10004008 |  14
0x10004004 |  99
0x10004000 |   7
```

3. Assume the base address is loaded into `$t4`.
   Write assembly code demonstrating two ways you could access `array[2]` in
   MIPS.
   *Hint*: One of the ways will require just one command,
   and the other will require more.

4. Assume the base address is loaded into `$t4`.
   Write assembly code to store the value 24 in `array[3]`.
   There are several ways to accomplish this.

5. Would writing general functions be possible without the `jal` instruction?
   If not, explain why not. If so, explain how.

6. Would the following function implementation and corresponding call work
   correctly?
   If not, why not?
   If so, is it a good implementation?

   ```
       addi $t0, $0, 4
       addi $t1, $0, 8
       jal sum            # sum(4, 8)
       ...

   sum:
       add $v0, $t0, $t1
       jr $ra
   ```

7. The following code does not work.
   Why? What would happen if it were run?

   ```
       # array entries are [1, 3, 9, 12, 15]
       # s0: base address of array
       # t0: constant 10
       # t4: accumulator
       addi $t0, $0, 10
       addi $t4, $0, 0

       lw $t1, 0($s0)

   loop:                    # loop while array entry < 10
       slt $t2, $t1, $t0
       beq $t2, $0, done
       add $t4, $t4, $t1    # $t4 += $t1
       addi $s0, $s0, 4     # move to next array entry
       j loop
   ```

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
