# QR-Code-Generator-using-Python

Project Summary 
Functionality: 
• QR Code Generation: The application allows users to generate QR codes by 
entering text data into an entry widget. 
• Visual Representation: Upon entering data and clicking the "Create" button, 
the application generates a QR code image based on the provided data. This 
image is displayed within the GUI. 
• Saving QR Codes: Users can save the generated QR code images to their 
desired location on their system by clicking the "Save" button. The application 
prompts the user to specify the file path and saves the image as a PNG file. 
• User Interaction: The GUI is designed with simplicity in mind, featuring 
intuitive buttons for creating, saving, and exiting the application. 
Structure: 
• Main Window: The application's main window is created using the Tkinter 
library, providing a clean and user-friendly interface for generating QR codes. 
• Entry Widget: Users input the data they want to encode into a QR code 
through an entry widget. 
• Buttons: The GUI includes three buttons: "Create", "Save", and "Exit". These 
buttons trigger corresponding actions such as generating QR codes, saving 
them, and exiting the application. 
• Canvas: The Canvas widget from Tkinter is utilized to display the generated 
QR code image within the application's GUI. 
Key Features: 
• Error Handling: The application includes error handling to ensure that users 
enter data before attempting to generate or save QR codes. 
GUI, enhancing visual appeal and readability. 
• Resizing: QR code images are resized to fit within the designated area of the 
the GUI elements according to their preferences. 
• Flexibility: Users have the flexibility to customize the size and appearance of 
• Feedback: The application provides informative messages via message boxes 
to notify users of successful operations or errors encountered during the 
process. 
Conclusion: In conclusion, this QR code generator application offers a convenient 
solution for creating and saving QR codes with ease. Its simple yet robust design 
makes it accessible to users of all levels, from beginners to experienced 
programmers. With its intuitive interface and essential features, the application 
serves as a valuable tool for various purposes, including information sharing, 
marketing, and more. 


Details of Process 
1. Import Libraries: 
• qrcode: This library is used to generate QR codes. 
• PIL: The Python Imaging Library is used for image processing, 
particularly for resizing the QR code image. 
• tkinter: This is the standard GUI (Graphical User Interface) toolkit for 
Python. 
• ttk, messagebox, filedialog: These are modules from Tkinter used for 
creating themed widgets, displaying message boxes, and handling file 
dialogs respectively. 
• createQR(*args): This function is called when the user wants to create a 
2. Define Functions: 
QR code. It retrieves the data entered by the user from the Entry widget 
(txt), generates a QR code image using the qrcode library, resizes the 
image using PIL, and displays it on the Canvas widget (qrc). 
• saveQR(): This function is called when the user wants to save the 
generated QR code image. It performs similar operations as createQR() 
but additionally prompts the user to choose a file path using a file 
dialog (filedialog.asksaveasfilename()) and saves the QR code image to 
the specified path. 
3. Create GUI: 
• Create a Tkinter root window (root) with a specific title, size, 
background color, and disabling resizing. 
• Create two frames (frame1 and frame2) within the root window to 
organize the layout. 
• Inside frame1, create a Canvas widget (qrc) to display the generated QR 
code. 
• Inside frame2, create an Entry widget (txt) for the user to input data, 
and three Button widgets (bt1, bt2, bt3) for creating the QR code, saving 
the QR code, and exiting the application respectively. 
• Place all the widgets and frames within the root window at specific 
positions using the place() method. 
4. Main Event Loop: 
interactions and responds accordingly. 
5. User Interaction: 
• Start the Tkinter event loop (root.mainloop()), which waits for user 
• The user enters data into the Entry widget (txt). 
• Clicking the "Create" button (bt1) or pressing Enter triggers the 
createQR() function, generating and displaying the QR code on the 
Canvas widget (qrc). 
• Clicking the "Save" button (bt2) triggers the saveQR() function, which 
saves the generated QR code image to a user-specified location. 
• Clicking the "Exit" button (bt3) exits the application. 
