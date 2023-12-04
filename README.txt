Kevin Wang - kw3020@nyu.edu

My code first puts all the instructions into the memory addresses. The simulation was done as a while loop that keeps read instructions until told not to.
Then does the execute_instruction function which decides which instrction to do. Within ther execute_instruction function, it calls all the other instructions that I wrote as seperate functions. It was easy to write out each instruction as it's own function. 
This kept things simple and organzied. Then in the execute_instruction function, all values were updated such as pc. In my jump conditional, I would first check to see if the jump was to the same addresses
to keep for a halt instruction. This would change the running variable to false which would end the simulation loop. I used a lot of uint16_t to avoid having troubles but then used int16_t with things that involed 2's comp and negative numbers.