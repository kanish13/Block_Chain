A struct is a creative data structure format in Solidity where variables of diverse data types can be bundled into one variable or a custom-made type.
 
To access any member of a structure, we use the member access operator (.). The member access operator is coded as a period between the structure variable name and the structure member that we wish to access.

Ex:

    // SPDX-License-Identifier: MIT
    pragma solidity >=0.8.8;

    contract test {
       struct Book { 
          string title;
          string author;
          uint book_id;
       }
       Book book;

       function setBook() public {
          book = Book('Learn Java', 'TP', 1);
       }
       function getBookId() public view returns (uint) {
          return book.book_id;
       }
    }
 
Output:

0:
uint256: 1
