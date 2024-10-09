# Telephone Directory in C++

This is a simple command-line telephone directory application written in C++ that allows you to manage contacts. The program enables you to add, search, view, delete, and update contact details. It uses file handling to store the contacts persistently.

## Features

- **Add Contact**: Add a new contact by providing a name, phone number, and email.
- **View All Contacts**: View all saved contacts in a neatly formatted table.
- **Search Contact**: Search for a contact by name or phone number.
- **Delete Contact**: Delete a contact by name or phone number.
- **Update Contact**: Update the contact information for an existing contact.

## Requirements

To run this project, you need the following:

- A C++ compiler (e.g., `g++` for Linux/Windows or Xcode for macOS)
- Basic knowledge of how to use a terminal or command prompt.

## Installation and Usage

1. **Clone the repository** (if applicable):
    ```bash
    git clone <repository_url>
    cd telephone-directory
    ```

2. **Compile the C++ code**:
    - On Linux/macOS:
      ```bash
      g++ TelephoneDirectory.cpp -o TelephoneDirectory
      ```
    - On Windows (if using `g++` from MinGW or Cygwin):
      ```bash
      g++ TelephoneDirectory.cpp -o TelephoneDirectory.exe
      ```

3. **Run the application**:
    - On Linux/macOS:
      ```bash
      ./TelephoneDirectory
      ```
    - On Windows:
      ```bash
      TelephoneDirectory.exe
      ```

4. **Use the Menu**:
    Once the program is running, you'll be presented with a menu where you can choose to add, view, search, delete, or update contacts. Follow the on-screen instructions for each option.

    Example of the menu:
    ```
    ==== Telephone Directory ====
    1. Add Contact
    2. View All Contacts
    3. Search Contact
    4. Delete Contact
    5. Update Contact
    6. Exit
    Choose an option:
    ```

## Project Structure

- `TelephoneDirectory.cpp`: Main program that handles all functionalities such as adding, searching, deleting, and updating contacts.
- `directory.txt`: The text file where all the contact data is saved. This file is created automatically when you add your first contact.

## How it Works

- **Adding a Contact**: When you add a contact, the information (name, phone, email) is appended to the `directory.txt` file.
- **Viewing Contacts**: The program reads the `directory.txt` file and displays all contacts in a formatted table.
- **Searching for a Contact**: The program reads the file and looks for a match based on either the name or the phone number.
- **Deleting a Contact**: The program creates a temporary file that excludes the contact you wish to delete, and then replaces the old file.
- **Updating a Contact**: The program finds the contact in the file, updates the details, and saves the changes by writing to the file again.

## Enhancements You Can Make

This project can be extended in several ways:
- Add input validation (e.g., ensuring phone numbers are numeric).
- Sort the directory alphabetically before displaying the contacts.
- Add more search functionality (search by email, partial matches, etc.).
- Implement a Graphical User Interface (GUI) using libraries like Qt or wxWidgets.

## Example Usage

Here’s an example of adding and viewing a contact:

1. **Add Contact**:
    ```
    Enter Name: John Doe
    Enter Phone: 123-456-7890
    Enter Email: john@example.com
    Contact added successfully!
    ```

2. **View All Contacts**:
    ```
    Name                 Phone          Email
    ---------------------------------------------------------------
    John Doe             123-456-7890   john@example.com
    ```

## Contributing

Feel free to fork this repository and contribute by submitting a pull request. Suggestions for improvements are welcome!

## License

This project is open-source and is licensed under the MIT License.
