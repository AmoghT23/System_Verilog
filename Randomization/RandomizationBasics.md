**Randomization**

Why?? \
-> Directed tests can take a long time and exhaustive testbenches are not always possible due to which there can be few cases which are not checked. \
-> With the help of constraints we can make a directed but random test case generation. This is called as Constrained Random Verification (CRV). \
-> Syntax - rand OR randc(cyclic random so the values will be repeated only when all the values are picked). \
-> We can ensure that we dont get any junk/garbage value by using 'assert()'. \
-> The randomization should be such that it should not contradict with the other cases. \ 
-> 'randomize()' function is used to invoke the part of the class object to randomize rand data type. \

"Prerandomize" \
-> The function which is used within the same class whose object will be randomized and called before "randomization". \

"Postrandomize" \
-> The function which is used within the same class whose object will be randomized and called after "randomization". \ 
-> If the randomization fails then we dont do the postrandomize.

"Override" \
-> Pre-randomize and post-randomize are not virtual, but behaves as virtual methods. (In case of manual then it will throw an compiler error). \
-> Before this the we used to override existing pre_randomize() and post_randomize() with our own definition. \

"rand_mode()" \
-> Can be called as both function and task. Current state of the variable will be returned if it is a called as a function. \

"rand_case()" \
-> Where we want the solver to randomly pick one out of many statements(states). \
-> This introduces a case statement that randomly selects one of its branches. The case item expressions are positive integer values that represent the weights associated with each item. \
-> Probability of selecting an item is derived by the division of that item's weight divided by the sum of all weights.  
