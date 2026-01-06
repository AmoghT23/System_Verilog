**Loops Basics**

1. Forever Loop
   -> This loop is same as while(1). \
   -> The simulation will hang unless you include the delay time inside the block to advance in the simulation time.

2. Repeat Loop
   -> Used to repeat statements in a block a certain number of times. \
   -> This is similar to for loop but in for loop we need another variable which increases the complexity. 

4. While Loop
   -> The simple loop which is true until the condition is true. \
   -> Example a counter which is incremental.

5. For Loop
   -> This mentions starting value, condition and incremental (or decremental) all in the same line. \
   -> j = i++ Post Increment, assign i to j and increment by 1 \
   -> j = ++i Pre Increment, increment 1 and then assign i to j \
   -> j = i-- Post Decrement, decrement i to j and then decrement by 1 \
   -> j = --i Pre Decrement, decrement 1 and then assign i to j 

6. Do While Loop
   -> This executes the code earlier and then it will check the condition to see if the code should be executed again.

7. For Each Loop
   -> Suitable for loop through array variables as we dont have to find the array size, set-up a variable to start from 0 to array_size-1 and increment it on every iteration.

8. Break and Continue
   -> break - The operation will break through the loop and go out to the next instruction(command/loop) \
   -> continue - Even if the conditions is satisfied or completed the loop will still be continued.

9. Unique Each/ Priority Each for fault checks
    -> unique-if - Evaluates if the conditions in any order reports an error when none if conditions match unless there is an explicit else. \
                   Report an error when there is more than 1 match found in the if else condition. \
    -> priority-if - Evaluates all the conditions in sequential order and a violation is reported when none of the conditions is true or if there's no else clause to the final if construct. \
    -> unique, unique0 - Ensures there is no overlapping in case items and hence can be evaluated in parallel. \
                         If more than one case item if found to match the given expression, then a violation is reported and the first matching expression is executed. \
                         If no case item is found to match the given expression, then a violation is reported only for unique. 
   
10. Always block (always, always_ff, always_comb)
    -> always - Used where combination and sequential elements can prove to be unstable or underperform due to limitations. Generic use and not a specific logic. \
    -> always_comb - Used when we have the intent to model a combinational logic and don't have to write a "sensitivity list" yourself. \
                      So the tool automatically works as a combinational logic. \
    -> always_latch - Used when we have the intent to model a latch-based logic. \
                      The variables assigned inside an "always_latch" block cannot be driven by other procedural block. \
                      This executes at time zero to make sure the latch consistent with the inputs at the very start of simulation. \
                      Don't have to write a "sensitivity list" yourself. \
    -> always_ff - A procedural blokc used to model synthesizable sequential circuits such as flipflops. \
                   This requires an explicit sensitivity list. This allows the designer to specify synchronous or asynchronous set/reset behavior. \
                   Removes the ambiguity and lets the designer design without any issue.  
