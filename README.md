# PASSWORD-MANAGER
This script creates a password manager using the Tkinter library in Python. Here's a breakdown of the key components:

1. Password Generator (generate_password):
   . It generates a random password by combining letters, numbers, and symbols.
   . The password has a random length: 8-10 letters, 2-4 symbols, and 2-4 numbers.
   . After generating the password, it shuffles the list of characters and joins them into a single string.
   .The generated password is inserted into the password entry field and copied to the clipboard using the pyperclip module.
2. Save Password Functionality (save):
  .This function retrieves data entered by the user (website, email, and password).
  .It validates that none of the fields are empty. If any field is empty, an error message is displayed using messagebox.showinfo.
  .The user is asked for confirmation before saving the details.
  .If confirmed, the data is appended to a file (data.txt) in the format: website|email|password.
 .After saving, the input fields for the website and password are cleared.
3. UI Setup:
  .The window is created using Tk() and configured with padding.
  .A logo image is displayed using a Canvas widget.
  .Labels are created for the website, email, and password fields.
 .Input fields (Entry widgets) are set up for the user to input the website, email, and password.
 .The password field allows the user to either enter a password or use the "Generate Password" button to create one automatically.
  .The "Add" button triggers the save() function to store the entered information.
