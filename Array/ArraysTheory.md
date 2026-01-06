**ARRAYS**

Static - Size of the array is known 

---Packed--- \
-> This type of arrays which are stored in consecutive spaces in the memory. \
->  [0][1][2][3][4][5][6][7] \
-> Used in the RTL design (ALU, Databus, Registers) \
-> Size known at the Compile Time  \
-> They can be single dimension, multidimensional \ 

---Unpacked--- \
-> This type of arrays which are stored in non consecutive spaces in memory. \
->  [][][][][][0]
    [][][][][][1]
    [][][][][][2]
    [][][][][][3]
-> Used in both RTL and Testbench. (Memories, FIFO, Register Files) \
-> Size known at the Compile Time \

Dynamic - Size unknown \

1. Dynamic
   -> This is an unpacked array whose size can be changed at the Run Time.
   -> Size of the dynamic array can be declared as new()
   -> Not Synthesizable so used in testbench ONLY. (Transaction Level Modelling)
   
2. Associative
   -> The items are stored in the form of key (generally the datatype).
   -> When the data is sparse no space is allocated until end.
   -> The items are accessed using arbitrary keys. (Reference Models, Tracking packets, RunTime).

3. Queue
   -> Non Synthesizable so used in Verification. (FIFO, Transaction Ordering, Stimulus, generator)
   -> Size at the Runtime
   -> Syntax type name [$:N] OR type name [$]
   -> We can perform operations like push and pop.   
    
