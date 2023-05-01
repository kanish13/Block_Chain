Step 1 − Write code in Remix IDE Code Section.

Example:

    pragma solidity ^0.5.0;
    contract SolidityTest {
       constructor() public{
       }
       function getResult() public view returns(uint){
          uint a = 1;
          uint b = 2;
          uint result = a + b;
          return result;
       }
    }

Step 2 − Under Compile Tab, click Start to Compile button.

Step 3 − Under Run Tab, click Deploy button.

Step 4 − Under Run Tab, Select SolidityTest at 0x... in drop-down.

Step 5 − Click getResult Button to display the result.

Output:

0: uint256: 3
