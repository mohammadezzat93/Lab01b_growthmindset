## JS Debugging

- Errors can (will) happen, every time you write some new computer code.

- Often, when programming code contains errors, nothing will happen. There are no error messages, and you will get no indications where to search for errors.

- Searching for (and fixing) errors in programming code is called code debugging.

- Searching for (and fixing) errors in programming code is called code debugging.

### JavaScript Debuggers
-Debugging is not easy. But fortunately, all modern browsers have a built-in JavaScript debugger.

-Built-in debuggers can be turned on and off, forcing errors to be reported to the user.

-With a debugger, you can also set breakpoints (places where code execution can be stopped), and examine variables while the code is executing.

### The console.log() Method

#### Definition and Usage
-The **console.log()** method writes a message to the console.

-The console is useful for testing purposes.

## Error Objects

![Image](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Errors-1200x720.jpg)

### **Error**

-Error objects are thrown when runtime errors occur. The Error object can also be used as a base object for user-defined exceptions

**Description**

-Runtime errors result in new Error objects being created and thrown.

### Error types
- Besides the generic Error constructor, there are other core error constructors in JavaScript. For client-side exceptions

**EvalError**  
Creates an instance representing an error that occurs regarding the global function eval().  

**RangeError**  
Creates an instance representing an error that occurs when a numeric variable or parameter is outside of its valid range.

**ReferenceError**    
Creates an instance representing an error that occurs when de-referencing an invalid reference.  

**SyntaxError**  
Creates an instance representing a syntax error.

**TypeError**  
Creates an instance representing an error that occurs when a variable or parameter is not of a valid type.  

**URIError**  
Creates an instance representing an error that occurs when encodeURI() or decodeURI() are passed invalid parameters.

**AggregateError**  
Creates an instance representing several errors wrapped in a single error when multiple errors need to be reported by an operation, for example by Promise.any().  

**InternalError**   
Creates an instance representing an error that occurs when an internal error in the JavaScript engine is thrown. E.g. "too much recursion".

## Browser Dev Tools & javascript console

### Debug JavaScript

#### Step 1: Reproduce the bug 

- Finding a series of actions that consistently reproduces a bug is always the first step to debugging.

#### Step 2: Get familiar with the Sources panel UI 

- DevTools provides a lot of different tools for different tasks, such as changing CSS, profiling page load performance, and monitoring network requests. The Sources panel is where you debug JavaScript.

#### Step 3: Pause the code with a breakpoint 
- A common method for debugging a problem like this is to insert a lot of console.log() statements into the code, in order to inspect values as the script executes.

#### Step 4: Step through the code #
- One common cause of bugs is when a script executes in the wrong order. Stepping through your code enables you to walk through your code's execution, one line at a time, and figure out exactly where it's executing in a different order than you expected. 

#### Step 5: Set a line-of-code breakpoint 
Line-of-code breakpoints are the most common type of breakpoint. When you've got a specific line of code that you want to pause on, use a line-of-code breakpoint

#### Step 6: Check variable values 
#### Step 7: Apply a fix 
You've found a fix for the bug. All that's left is to try out your fix by editing the code and re-running the demo. You don't need to leave DevTools to apply the fix. You can edit JavaScript code directly within the DevTools UI.