📱 Contact Manager Application (Python)
This is a simple Contact Manager application built in Python. It allows users to add, view, update, delete, and search contacts. The program stores the contacts in a dictionary, where each contact consists of a name, phone number, and email address.
________________________________________
🎯 Features
    •	Add contact: Input a name, phone number, and email to add a contact.
    •	View all contacts: List all saved contacts with their details.
    •	Update contact: Modify an existing contact’s number and/or email.
    •	Delete contact: Remove a contact from the list.
    •	Search contact: Find a contact by name.
    •	Clear screen: After each action, the screen is cleared to keep it clean.
________________________________________
🛠️ Requirements
•	Python 3.x (compatible with any ve  rsion of Python 3.x)
________________________________________
🚀 How to Run
    1.	Clone or Download the repository.
    2.	Ensure that you have Python 3 installed on your system.
    3.	Open a terminal and navigate to the folder containing the script.
    4.	Run the script using:
            python contact_manager.py
    5.	Follow the prompts to manage your contacts.
________________________________________
🧠 Code Structure
1. Contacts Dictionary
  •	The contacts are stored in a dictionary where the key is the contact's name, and the value is a list containing the phone number and email.
2. Action Menu
The user is presented with an action menu to:
  •	Add a contact (a)
  •	Open (view) all contacts (o)
  •	Update a contact (u)
  •	Delete a contact (d)
  •	Search for a contact (s)
  •	Quit the application (q)
3. Functionality
  •	Add Contact: Prompts the user for a name, number, and email, then adds it to the dictionary.
  •	Open All Contacts: Displays all saved contacts.
  •	Update Contact: Prompts the user for a contact name and updates their number and/or email.
  •	Delete Contact: Removes a contact based on the given name.
  •	Search Contact: Searches for a contact by name and displays their details if found.
  •	Exit: Exits the application.
4. Clear Output
  The output is cleared after each action using clear_output(wait=True) to maintain a clean interface.
________________________________________
📚 What I Learned
While working on this project, I learned:
  •	How to manage user input and provide meaningful feedback.
  •	How to use dictionaries in Python to store and manage data.
  •	Techniques for validating user input and handling errors gracefully.
  •	How to clear the console screen for a clean user interface using clear_output(wait=True).
This project improved my understanding of basic Python concepts like dictionaries, loops, and conditional statements.
________________________________________
🚀 Future Improvements
    •	Add validation to ensure the phone number and email follow proper formats. (Using Regex)
    •	Allow saving the contacts to a file (e.g., JSON, CSV) for persistence.
    •	Implement password protection or a simple login system to access the contact manager.
    •	Provide an option to export contacts to a file (e.g., CSV, JSON).

Using Regex
Yet another problem with our app is "lack of validation". While creating a new contact, user is free to enter anything. But why is that a problem?

**Input validation** is important to ensure only properly formed data is entering the workflow in an information system, preventing malformed data from persisting in the database and triggering malfunction of various downstream components. Input validation should happen as early as possible in the data flow, preferably as soon as the data is received. [source](https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html)

The above paragraph is the complete gist of Input validation. Read it again & ponder for a minute. Its an important concept when building customer facing applications. We would highly recommend you to Google and read more about it.  

Use regular expression to validate user input (before you save it to the file). Implement the following:
    •	`Name` should be all alphabets. " " should also be allowed.
    •	For `email` refer regex chapter from course material.
    •	`Number` should have 10 digits. Not less, not more. Also, not alphabets should be allowed.
    •	Add a new field `DOB` to each contact. It should follow YYYY-MM-DD format. Then write a regular expression to validate it. Remember, date & month cannot be greater that 31 & 12, respectively.


