
#############################################################
ReadMe for assignment submitted by 2019B5PS0658P
Practical section number: P6
Asignment question attempted: 2
#############################################################
Team:
1. 2019A2PS0830P   Aayush
2. 2019B5PS0658P TANISH
#############################################################
Description of how to run the code and observe the output
1. The .c is called 2019B5PS0658P_P6.c. It is a menu-driven application.staff username is user and password is 123, please make your own student account from staff login. code is not compatible in windows
2. The input files are :-
Main Database Files: -
	AUTHOR.txt = Contains the name of all the book’s author present in the library inventory
	Count.txt = Contains the total number of a particular title available in the library inventory
	Genre.txt = Contains the genre of a particular title available in the library inventory
	Issue_no.txt = Issue number of all the books available in the library
	Liblist.txt = List of all the libraries that we can request books from
	TITLE.txt = List of titles of all the books present in the library inventory
	Total.txt = Stores the total count of books present in the library
	Vendor.txt = List of all the vendors from whom we can order books
        ps_rqt = files related password reset request
User Management: -
	FacultyDob.txt = Stores the DOB of all the faculty members who are registered to the library
	FacultyId.txt = Stores the ID of all the faculty members who are registered to the library
	FacultyName.txt = Stores name of all the faculty members who are registered to the library
	FacultyPass.txt = Stores the pass of all the faculty members who are registered to the library
	StaffDob.txt = Stores the DOB of all the staff members who are registered to the library
	StaffId.txt = Stores the ID of all the staff members who are registered to the library
	StaffName.txt = Stores the name of all the staff members who are registered to the library
	StaffPass.txt = Stores the password of all the staff members who are registered to the library
	StudentDob.txt = Stores the DOB of all the student members who are registered to the library
	StudentId.txt = Stores the ID of all the student members who are registered to the library
	StudentName.txt = Stores the name of all the student members who are registered to the library
	StudentPass.txt = Stores the pass of all the student members who are registered to the Library
Issued Book Details: -
	IssuedBooks.txt = Stores the issue no. of all the issued books
	IssuedOnDate.txt = Stores the date on which the book was issued
	IssuedUserId.txt = Stores the ID of the person who issued the book	
Reserved Book Details: -
	ReservedBooks.txt = Stores the issue no. of the reserved books
	ReservedUserId.txt = Stores the ID of the person who reserved the book
Requested Book Details: -
	RequestedAuName.txt = Stores the name of the author of the book one request
	RequestedTitle.txt = Stores the title of the book requested
	RequestedUserId.txt = Stores the ID of the person who request book
	ApprovedRequestAuthor.txt = Stores the author of the book’s request that are approved by staff
	ApprovedRequestTitle.txt = Stores the title of the book’s request that are approved by staff
	ApprovedRequestUserId.txt = Stores the ID of the person whose book request is approved by author
Order Book Details: -
	Authorodr.txt = Stores the author name of the book which is ordered by staff
	booknameodr.txt = Stores the title of the book which is ordered by staff
	genreodr.txt = Stores the genre of the book which is ordered by staff
	orderid.txt = Stores the order ID of the books
	qtyodr.txt = Stores the number of particular titles ordered by staff
	statusodr.txt = Stores the status of the book that is ordered by staff
	vendorodr.txt = Stores the name of the vendor/library from where book is ordered/requested
	
Cart: -
	CartBooks.txt = Stores the issue no of the book that is added to cart
	CartUserId.txt = Stores the ID of the person who added a particular title


Working of the Program:-
When you start the application, you will be prompted to the screen where you will be asked to select one of the following options: Sign in/ Sign Up/ Exit
If any new book is added, an alert is also displayed on the same screen.
Sign in will prompt the Login portal whereas Sign up will tell you how to get membership and Exit as will close the application.

Login screen will have the following options: Student/Staff/Faculty
Student-Students who are registered to the library can login through this menu
Faculty-Faculty who are registered to the library can login through this menu
Staff- Staff who are managing the library portal can login through this menu

Login will ask for two fields, UserID and Password, on entering any of the field incorrectly, you will be asked whether you want to input the fields again or want to change the password.

On choosing password change option, you will have to enter your UserID, if exists, will ask for DOB for security purposes and the new password you want to have else will tell UserID doesn’t exist.
On getting all the fields, will redirect you to login screen. One cannot login with the new password unless someone from the staff accept the request.
One cannot enter password change request more than once unless the staff accept/decline the previous request.
On successfully signing in, (through student/faculty) an alert is shown if any of the requested /reserved book is available in the library, and also a reminder to return a book if its been issued for more than 15 days.

Student Portal: -
Issue Book: -
To issue a book, you are required to search it. The search function is made in such a way that it will search across all the fields i.e., TITLE, AUTHOR, GENRE, Issue No. all at once and also if you want to search a book which whose title is “SLAUGHTERHOUSE FIVE”, you can just search for this by typing “house” without taking care of the case sensitivity, the required book will be in one of the results found. 
After selecting a particular book, you can either issue it right away, put it into cart or search books by same author.
If the book is available in the library, but the count of the book is 0, then you can put a request to reserve the book so that when the book is available, you will be notified. Once the book is back in the inventory, you can go to cart and order it through there. Once you visit cart and do not order the book, the reservation is deleted.
If the book is not available in the library, you can request the book to add in the library. 

Here we tried to add a new feature, that when the book is added it will automatically be added to the cart. But this is not functioning completely.

Return Book: -

It will list all the books that one has issued so far and will take the input of the serial no of the book that has been returned.

Staff Portal: - 

Add Member: -
This option adds the member by asking which type of account you want to add.
You are supposed to enter userID and password and DOB and name of the person whose account is to be added

Delete Member: -
This option helps to delete a certain member by taking the type and its userID

Inventory: - 
This is a menu in itself which has all the options regarding orders, and books.
It helps staff to add/delete books, process orders, show who has order which book, and also current count of particular title.


Add Book(s): -

To add a book, user gets two option. 1) search by issue no - using this option user can directly increase count (or quantity) by 1 of existing books in library by searching through issue no.
2)search by title, author, book name- using this option user can search book and select serial no. to increase book count (or quantity) by 1 of existing books in library, and if no results are found in search then a prompt will ask user to enter details of author, title, genre and add a book with default count (or Quantity) of 1.


Delete Book(s): -
To delete a book, user gets two option. 1) search by issue no - using this option user can directly decrease count (or quantity) by 1 of existing books in library by searching through issue no.
2)search by title, author, book name - using this option user can search book and select serial no. to decrease book count (or quantity) by 1 of existing books in library.


Order Book(s): -
In order Menu user gets 3 option to choose from 
1.Place Order
2.View Order
3.Manage order
On selecting 1 option user gets choice to order books through different Vendors/libraries then after user can choose a Vendor/library to place an order. After that a prompt appears which asks further details such as author, title, genre, quantity and checks if an duplicate order exists then asks user Yes/No to place order and if no duplicate order exists then directly places order.
On selecting 2 option user gets choice to view past orders, can select (1) to view all past orders (2) to view orders with current status as 'PENDING' (3) to view orders with current status as 'CANCELLED' and thus after selecting anyone of three users can view details to past orders.
On selecting 3 option user need to enter 'order id' now order details corresponding to this order id are displayed and a menu is appears which asks user to select one option to change current order status to 'PENDING','CANCELLED ‘ or 'RECEIVED' ,now if user selects  to change status to 'PENDING' or 'CANCELLED' it simply changes current order status whereas if user selects 'RECEIVED' option then this book details are further added to main database to library. 


Check Password Change Request: -

This shows the list of all the users who have requested to change their passwords. You can either accept/decline the request based on whether the DOB which was entered while creating the account and the one which was asked by the user while requesting the change request matches or not.
On decline, the password remains same where on accepting, It changes the password to the new one.
 
Check Book Requests: -

It shows list of all the books that has been requested by the student/faculty
You can order the books that are requested from here.



############################################################
Known limitations of the code :
1.	When adding/deleting book, one should not enter issue no greater than the number of available in to files
2.    Requested book when added to the library cannot be ordered directly through cart but can	 be searched and issued.
3.    When you have processed all the orders, and still try to view orders, you may get       
        Segmentation fault 
#############################################################
Countributed by Aayush and Tanish 
#############################################################
