DETAILS IN PARTS -

 1) PART A - 

 dictn = {}: Initializes an empty dictionary to store contacts.

Format will be like: {"John": [1234567890, 9876543210]}

inp = input(...): Takes the first operation from the user (add, search, delete, etc.).

 2) PART B - 

 add(name, num): Adds a number to the contact name.

If the name already exists, appends the number.

Otherwise, creates a new entry with the number in a list.

delete(name): Deletes the contact if it exists, otherwise prints an error.

search(name): Searches and displays all numbers saved for that name.

prin(): Prints the entire contact book (the dictn dictionary).

 3) PART C -

 A loop that continues until the user types "exit".

Based on user input (add, search, delete, print), it:

Asks for more input (name, number).

Calls the corresponding function (add, search, etc.).

After every operation, it asks again for the next operation.

ERRORS I FACED -
 
1) Local vs Global dictionary:
In the add() function, 1 wrote dictn = {name:num} which redefines the dictionary locally, so it doesn't affect the global dictn.

2) Appending to a non-list:
I tried dictn[name].append(num) right after assigning dictn = {name:num} — but num is an int, not a list. Integers don’t support .append().

3) inp only asked once:
I only asked for the operation once, so the loop didn’t update the input unless the program was restarted.
