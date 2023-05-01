A function is a group of reusable code which can be called anywhere in your program. This eliminates the need of writing the same code again and again. It helps programmers in writing modular codes. Functions allow a programmer to divide a big program into a number of small and manageable functions.

Syntax:

    function function-name(parameter-list) scope returns() {
       //statements
    }
    
 Ex:
 
     contract Test {
       function getResult() public view returns(uint){
          uint a = 1; // local variable
          uint b = 2;
          uint result = a + b;
          return result;
       }
    }
