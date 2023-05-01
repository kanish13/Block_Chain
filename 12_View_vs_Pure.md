View:

It only reads the state variable and not modify.

Ex:

    pragma solidity >=0.8.8
    contract a{
    int public num;
    function b() public view returns (int){
    return num;
    }
    }
    
Pure:

It neither read nor modify the state variable.


Ex:

    pragma solidity >=0.8.8
    contract a{
    int public num;
    function b() public pure returns (int){
    return 1;
    }
    }
