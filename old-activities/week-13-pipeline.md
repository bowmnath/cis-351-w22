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

1. Work through the questions in the
   [caches and block size handout](/misc/block-cache-handout.pdf)

2. Which of the following code snippets would most likely benefit most from
   the presence of a cache?
   Why?

   ```python
   total = 0
   for i in range(100):  # for (int i = 0; i < 100; i++)
       total += 5
   ```

   ```python
   total = 0
   for i in range(100):
       total += array[i]
   ```

   ```python
   total = 0
   for j in range(25):
       for i in range(4):
           total += array[i]
   ```

3. Give an example of code (assembly or high-level) where spatial locality
   applies,
   but temporal locality does not (or does not much).

4. Give an example of code (assembly or high-level) where temporal locality
   applies,
   but spatial locality does not (or does not much).

5. Consider the following sequence of cache hits and misses.
   What is the average memory access time assuming a cache access costs 1 ns
   and a memory access costs 500 ns?
   What would the average memory access time be without a cache?

   H, M, M, M, H, H, H, H, H, H

6. Is it ever possible for memory and cache to be out of sync
   (i.e., the contents of memory are different from the corresponding cache
   entries)?
   If so, how can this happen?
   If not, why not?

7. Give an example of what could go wrong in a pipelined processor if the
   control signals were not pipelined as well.

8. The pipelined MIPS process we learned about in lecture has 5 stages.
   If we added a 6th stage,
   would throughput be improved?
   Why or why not?
   What about latency?

9. With a five-stage pipeline,
   how many instructions will the processor complete in the first 8 cycles?

10. With a five-stage pipeline and a clock cycle of 200 ps,
    what is the long-term throughput of the processor?
