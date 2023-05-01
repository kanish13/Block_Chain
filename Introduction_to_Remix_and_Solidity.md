Remix Online IDE is a powerful toolset for developing, deploying, debugging, and testing Ethereum and EVM-compatible smart contracts. It requires no setup and has a flexible, intuitive user interface. Start coding online.

Link: https://remix.ethereum.org/

![sol](https://user-images.githubusercontent.com/111358462/235410967-5b7c4c83-163b-447a-ae79-0794603cd3e2.png)

To compile and run program : CTRL+S

Solidity is an object-oriented programming language for implementing smart contracts on various blockchain platforms, most notably, Ethereum.

Get started:

* Go to remix website
* Create use file with your convinient name with extension .sol [ EX: simple.sol ]
* Type the following two lines of code which tells us to makes license and tells you the version solidity:

      // SPDX-License-Identifier: MIT
      pragma solidity 0.8.8;
 
 To create contract :
     
     contract SimpleSorage
     {
     }

Datatypes of Solidity:

Signed integers:

A signed integer, declared with the int keyword, is a value data type that can be used to store either positive or negative values in smart contracts.

int is an abbreviation for int256, which has a range of -2 ** 255 to 2 ** 255 - 1. This value type takes up to 32B by default, but we can make it smaller by specifying the number of bits in steps of 8. For example: int8, int16, int32, etc.

Unsigned integers:

An unsigned integer, declared with the uint keyword, is a value data type that must be non-negative; that is, its value is greater than or equal to zero.

uint is an abbreviation for uint256. Just like signed integers, this value data type takes up to 32B by default. Again, we can make it smaller by specifying the number of bits in steps of 8. For example: uint8, uint16, uint32, etc.

These integers are restricted to a range based on their size. For example, uint8 has a range of 0 to 2 ** 8 -1, and uint256 has a range of 0 to 2 **256 - 1.

Boolean:

The bool value data type is used in Solidity to illustrate cases that have binary results. A bool has two fixed values: true or false, with false being the default. This data type only takes up 1B of storage.

Solidity supports all standard Boolean operators, such as:

!= (inequality)

== (equality)

! (logical negation)

&& (logical conjunction, “AND”)

|| (logical disjunction, “OR”)

It is essential to understand that you cannot translate the bool data type into integers in Solidity like you would with other programming languages. Also, in Solidity any assignments to other Boolean variables creates a new copy of the variable.

Addresses
An address value type is specifically designed to hold up to 20B, or 160 bits, which is the size of an Ethereum address.

Solidity actually offers two address value types: address and address payable. The difference between the two is that address payable can send and transfer Ether.

We can use an address to acquire a balance using the .balance method and to transfer a balance using the .transfer method.

Bytes:

In Solidity, byte refers to 8-bit signed integers. Everything in memory is stored in bits with binary values 0 and 1.

Example:

    // SPDX-License-Identifier: MIT
    pragma solidity >=0.8.8;

    contract SimpleSorage{
        uint a=5;
        bool b=true;
        string c="five";
        int d=-7;
        address e=0x8e1103d379303b7bdF78d74358a306C01eD881B2;
        bytes f="cat";

    }

     
    

