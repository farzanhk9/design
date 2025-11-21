import tkinter as tk

# Create the main window
root = tk.Tk()
root.title("Simple Design Window")
root.geometry("400x300")  # Window size

# Create a label
label = tk.Label(root, text="Hello! Welcome to Tkinter Design", font=("Arial", 14))
label.pack(pady=20)  # Position the label with vertical padding

# Function to change the label text
def change_text():
    label.config(text="Text has been changed!")

# Create a button
button = tk.Button(root, text="Change Text", command=change_text, font=("Arial", 12))
button.pack(pady=10)  # Position the button with vertical padding

# Start the main loop of the program
root.mainloop()
