This code produces a library management system. 
It comes in three classes, followed by a set of functions for the GUI.

 ![Screenshot (103)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/301bf5a3-55f0-47ee-a9ad-93eb1469c14d)

In order to use it:
-run the code

-click "register here" and input your name and contact information, or any shortened form, then click on the prompt. This will allow you to take out and return books.

-type "sudo" into the lower textbox and click the label above it to access the full suite of features, including the ability to add books. Change the entered password to something else and click again to lock down these features again.

-most buttons are obvious. Some require the central "ISBN" field to be filled, or the "PatronID" field in the top right. If this is not filled, they will give you a popup telling you to check your inputs.

-click on popups to dismiss them.

-"write off a book" removes a copy of a book, and all info tied to that copy, from the system. If a PatronID is entered, it will attempt to delete the book in that Patron's posession. Otherwise, it removes one from the 'shelves'.

-click "save data" to save all books,patrons,and due dates to your computer. They will be automatically downloaded when you next open the program.

![Screenshot (86)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/22225700-28a6-4713-933b-9c5b96c5984a)
![Screenshot (87)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/fcd8193c-e6d1-405f-9244-aac62242415d)
![Screenshot (88)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/983195b1-fe08-4880-b6a1-ded64be24fa8)
![Screenshot (89)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/4e263314-afad-42a2-98fc-bb38fc7f2beb)
![Screenshot (90)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/8beaca91-3e30-40bf-b863-0372ba36ff9d)
![Screenshot (91)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/bbbab084-9ad9-4c8c-8cdf-61a59efa706a)
![Screenshot (92)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/4eed853b-d949-47ad-b034-d8553ed33265)
![Screenshot (93)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/d5b6537b-68d6-45ac-ba08-7101dae65421)
![Screenshot (94)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/0e7ce941-60f1-4290-b330-3eafd5670853)
![Screenshot (95)](https://github.com/Glory-Be-Upon-Me/Repository/assets/162057176/9129deda-53ae-47de-86c7-bb82e737e22e)
...You get the idea.

While writing this, I learned to automate the creation of class objects using exec(), and to use the tkinter module to create a GUI. One of my main challenges was that creating a class requires a variable to hold it, and I had no way of automatically generating and using new ones until I learned to use exec() and eval(). 
I also had to deal with many errors, like missing apostrophes and, at one point, accidentally referencing the _selected_ ISBN instead of the one I was displaying. However, I was able to find all of them.

This code is likely vulnerable to injection attacks, and the admin password cannot be changed without going into the code and editing it. Additionally, some of the early functions are written sloppily and are unnecesarily long. 

Also, you can find the admin password by just reading the source code. That's probably a security vulnerablity.

If I were writing it again, it would probably be more tidy and consistent.
