import tkinter as tk
from tkinter import ttk

def add():
    """Addition"""
    result = float(num1_entry.get()) + float(num2_entry.get())
    result_label.config(text="Result: " + str(result))

def subtract():
    """Subtraction"""
    result = float(num1_entry.get()) - float(num2_entry.get())
    result_label.config(text="Result: " + str(result))

def multiply():
    """Multiplication"""
    result = float(num1_entry.get()) * float(num2_entry.get())
    result_label.config(text="Result: " + str(result))

def divide():
    """Division"""
    try:
        result = float(num1_entry.get()) / float(num2_entry.get())
        result_label.config(text="Result: " + str(result))
    except ZeroDivisionError:
        result_label.config(text="Error! Division by zero!")

# Create the main window
root = tk.Tk()
root.title("Calculator")

# Styling
root.geometry("425x200")
root.configure(bg='#f0f0f0')
root.resizable(False, False)

# Create entry widgets for numbers
num1_entry = ttk.Entry(root, width=10, font=('Arial', 12))
num1_entry.grid(row=0, column=0, padx=10, pady=10)

num2_entry = ttk.Entry(root, width=10, font=('Arial', 12))
num2_entry.grid(row=0, column=2, padx=10, pady=10)

# Create labels for the entry widgets
ttk.Label(root, text="Number 1", font=('Arial', 12), background='#f0f0f0').grid(row=0, column=1, padx=10, pady=10)
ttk.Label(root, text="Number 2", font=('Arial', 12), background='#f0f0f0').grid(row=0, column=3, padx=10, pady=10)

# Create buttons for operations
button_style = ttk.Style()
button_style.configure('TButton', borderwidth=0, relief="flat", background='#0080ff', font=('Arial', 12))

add_button = ttk.Button(root, text="+", command=add, style='TButton')
add_button.grid(row=1, column=0, padx=10, pady=10)

subtract_button = ttk.Button(root, text="-", command=subtract, style='TButton')
subtract_button.grid(row=1, column=1, padx=10, pady=10)

multiply_button = ttk.Button(root, text="*", command=multiply, style='TButton')
multiply_button.grid(row=1, column=2, padx=10, pady=10)

divide_button = ttk.Button(root, text="/", command=divide, style='TButton')
divide_button.grid(row=1, column=3, padx=10, pady=10)

# Label to display result
result_label = ttk.Label(root, text="Result:", font=('Arial', 12), background='#f0f0f0')
result_label.grid(row=2, columnspan=4, padx=10, pady=10)

root.mainloop()

