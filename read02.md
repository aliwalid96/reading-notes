## Unit tests
Arrange, Act and Assert.
1. you need to organize the data needed to execute that piece of code (input);
2.  here you will execute the code being tested (exercise the behaviour);
3. after executing the code, you will check if the result (output) is the same as you were expecting.
### The Cycle
The cycle is made by three steps:
1. Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
2.  Write the feature and make the test pass! (you can dance after that)
3.  Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)
### TDD is not about the money/tests
 just building what is needed to make the test pass.
 When we are writing tests we are forced to think about the design first and how we can break it into small pieces
 ## What does the if __name__ == “__main__”: do?
 this will work only when you excute the code from main 


 Before executing code, Python interpreter reads source file and define few special variables/global variables

 A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. 
 thi

## Recursion

is The process in which a function calls itself directly or indirectly 
like this example 
int fact(int n)
{
    if (n < = 1) // base case
        return 1;
    else    
        return n*fact(n-1);    
}

