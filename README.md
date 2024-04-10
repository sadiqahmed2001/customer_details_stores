# customer_details_stores
simple address book management system. It allows users to add contacts with details such as name, phone number, email, and product, and also to display the existing contacts.

To begin, include the essential header files: <stdio.h> for standard input-output routines and <string.h> for string manipulation.

The program defines the constant MAX_CONTACTS, which specifies the maximum number of contacts that may be saved.


A structure called Contact is defined to store data about a single contact. It has fields for name, phone, email, and product.

Function prototypes for addContact and displayContacts are defined. These routines appear later in the code.


In the primary function:

It specifies an array of Contact structures named contacts, which may hold up to MAX_CONTACTS contacts.
It initializes the variable numContacts, which keeps track of the current number of contacts recorded.

It presents a menu of alternatives from which the user may select: add a contact, view contacts, or quit.
It reads the user's selection and executes the appropriate action using a switch statement.
The cycle will continue until the user chooses to exit.

The AddContact function:

Checks whether there is enough space in the address book (numContacts is fewer than MAX_CONTACTS).
If there is enough space, it prompts the user to input contact information for a new contact (name, phone number, email, and product) using scanf.

It increases the numContacts variable to indicate the insertion of a new contact.
If the address book is filled, the user is notified that no new contacts may be added.
DisplayContacts function:

Checks whether any contacts are saved (numContacts is not 0).
If there are no contacts, it produces a notice stating that the address book is empty.
If there are any contacts, it uses a loop to print out the information for each contact in the array.

The application provides a simple interface for managing contacts, allowing users to create new contacts and view current ones. However, it lacks input validation, error management, and other capabilities such as contact editing and deletion, all of which might be added to increase utility and robustness.
