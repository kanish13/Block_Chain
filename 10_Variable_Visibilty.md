
Public − Public state variables can be accessed internally as well as via messages. For a public state variable, an automatic getter function is generated.

Internal − Internal state variables can be accessed only internally from the current contract or contract deriving from it without using this.

Private − Private state variables can be accessed only internally from the current contract they are defined not in the derived contract from it.

Ex:

    // SPDX-License-Identifier: MIT
    pragma solidity >=0.8.8;

    contract SimpleStorage{
        int public x=30;
        int internal y=20;
        function store() public pure returns(int)
        {
            int b=5; //Private
            return b;
        }
         function func() public view returns(int){
            return y; //Internal
        }
    }
    contract sample {
        SimpleStorage v=new SimpleStorage();
        function fun() public view returns(int){
            return v.x(); //External
        }
    }
    
 Output:
 
 ![out](https://user-images.githubusercontent.com/111358462/235451951-5d9ea0fe-55c9-4d68-97cc-29d08a6359c7.png)
