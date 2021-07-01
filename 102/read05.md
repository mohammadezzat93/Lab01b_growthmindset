# Summary of today's lecture

# Operators and Loops

## Loop :  When you want to repeat somthing


1- **While :** We dont no how any time the code will run , but for sure we know it well keep running as long as the condition is true . 

2- **For :** We are gonna use When we know how many time the code need to run .  
  
- ## The while() loop

The while() loop has the form:

  while ( expression ) {  
    /* Do something... */  
  }  
  - **The contents of the loop, which as always may be a single statement or a { ... } block, are executed for as long as the controlling expression is true.**  

 - *If the condition is false the body of the loop never executes at all.
This may sound slightly unintuitive (if there's nothing to do, why have a loop?) but when writing a program we often don't know if there will always be something to loop over and it would be really inconvenient to have to wrap every loop inside an if() statement.*  

**Key Point : **If the condition is false the body of the loop never executes at all.  

- ## The for() loop  

The for() loop rolls all these three into one. It has the following format:

for (Initialise; Test; Increment ) {  
    ... /* Loop body */  
  }  

  - **Note that the three expressions are separated by semicolons, not commas, and that they occur in the same order as they are used. **  
- *The steps in the for() loop are done in exactly the same order as in the equivalent while() loop:*  

**Key Point : **
Initialise  
Loop:  
1-Test and if false quit the loop.  
2-Execute the body.  
3-Increment.