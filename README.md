This code produces a library management system. 
It comes in three classes, followed by a set of functions for the GUI.
 |_____________________
 |-
 |-
 |--- class 1(Book)
 |  --
 |  --functions
 |  --
 |--- class 2(Patron)
 |  --
 |  -- functions
 |  --
 |--- class 3(Transaction)
 |  --functions
 |  --
 |--save function
 |--
 |--
 |--functions for GUI 
 |--
 |--
 |-
 |-initialize GUI
 |-
 |____________________
In order to use it:
-run the code

-click "register here" and input your name and contact information, or a shortened form, then click on the prompt. This will allow you to take out and return books.

-type "sudo" into the lower textbox and click the label above it to access the full suite of features, including the ability to add books. Change the password to something else and click again to lock down these features again.

-most buttons are obvious. Some require the central "ISBN" field to be filled, or the "PatronID" field in the top right. If this is not filled, they will give you a popup telling you to check your inputs.

-click on popups to dismiss them.

-"write off a book" removes a copy of a book, and all info tied to that copy, from the system. If a PatronID is entered, it will attempt to delete the book in that Patron's posession. Otherwise, it removes one from the 'shelves'.

-click "save data" to save all books,patrons,and due dates to your computer. They will be automatically downloaded when you next open the program.

