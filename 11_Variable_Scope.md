Local Variable:

Local variables are declared within a function and are only accessible within that function. Their scope is limited, and their lifetime ends when the function execution is completed.

EX:

    pragma solidity ^0.8.0;

    contract LocalVariableExample {
      function getDouble(uint value) public pure returns (uint) 
      {
        uint doubleValue = value * 2;
        return doubleValue;
      }
    }

![1](https://user-images.githubusercontent.com/111358462/235455065-7caa002e-db36-4048-b7eb-08edcfd6d34c.png)

State Variable:

State variables are declared at the contract level and represent the contract’s state on the blockchain. They are stored on the Ethereum network and are accessible within the entire contract.

Ex:

    pragma solidity ^0.8.0;

    contract StateVariableExample {
      uint public count = 0;
      function increment() public 
      {
        count += 1;
      }
    }
    
![2](https://user-images.githubusercontent.com/111358462/235455401-699e9738-9edf-429d-99d7-afbe1e5e7740.png)

Global Variable:

Global variables are special variables provided by the Solidity language. They are available throughout the contract and provide information about the blockchain, transaction, and execution context.

    pragma solidity ^0.8.0;

    contract GlobalVariableExample {
      event SenderAndValue(address sender, uint value);
      function getSenderAndValue() public payable 
      {
        address sender = msg.sender;
        uint value = msg.value;
        emit SenderAndValue(sender, value);
      }
    }



