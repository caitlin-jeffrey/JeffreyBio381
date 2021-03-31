## Anatomy of a User-defined Function

```R
functionName <- function(parX=defaultX, parY=defaultY){
	# curly bracket marks start of function body
	# lines of R code and annotations
	# may also call other functions within this function
	# may also create functions within function
	# may define local variables - only live within the function itself
	
	return(singleObject) # returns a single object (could be a list)
    }

# curly bracket marks the end of the function body

functionName # print the function body
functionName() # run function with default values
functionName(parX=myMatrix, parY="Order", parZ=c(0,3,3,4))
	
```

## Stylistic Conventions for Writing Functions

- Use prominent hash character fencing at start and finish
- Give a header with function name, description, and inputs and outputs
- Names inside a function can be fairly short and generic
- Functions should be short and simple, no more than about a screenful
- If too long or complex, break it up into several functions
- Provide default values for all function arguments
- Ideally, use random number generators as default values for rapid testing

## Scoping

- Global variables visible to all parts of the code; declared in the main body
- Local variables visible only within a function; declared in the function or passed to the function through the parameters
- Functions can "see" global variables, but should not use them
- Global environment cannot "see" variables in the function environment
- "What happens in the function stays in the function"