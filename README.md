# Anaconda 1.0

Anaconda is a compiled programming language that was written in C++. It can compile Python Files and HTML files.

# Setup

1. Download the release tag.

2. Make a file that ends with .ana

   Here is the example code
   ```python
   print "Hello World!"
   print "Goodbye World!"
   ```

3. After writing the ```.ana```, now its time to compile. Type this command in the folder and make sure that an app called Anaconda.exe must installed.
  ```bash
  ./Anaconda example.ana -o example.py
  ```

4. Run the ```.py``` file

If you have some issues contact us at mmbkmcgamming2014@gmail.com!


# How to build an application in Anaconda

To build an Appilcation in Anaconda you must type this code inside your `.ana` code

```python
# Import tkinter for GUI window
import tkinter as tk

# Define the function to greet and calculate birth year
def greet():
    # Get the name and age from input
    let name = name_entry.get()
    let age = age_entry.get()
    
    # Create greeting and birth year messages
    let greeting_message = "Hello, " + name + "!"
    let birth_year = 2025 - toInt(age)
    let birth_message = "You were born in the year: " + birth_year

    # Update the labels with the greeting and birth year
    greeting_label.config(text=greeting_message)
    birth_label.config(text=birth_message)

# Create the main window
let window = tk.Tk()
window.title("Anaconda User App")

# Create labels and entry widgets for user input
let name_label = tk.Label(window, text="Enter your name: ")
name_label.pack()

let name_entry = tk.Entry(window)
name_entry.pack()

let age_label = tk.Label(window, text="Enter your age: ")
age_label.pack()

let age_entry = tk.Entry(window)
age_entry.pack()

# Create button to trigger the greeting function
let greet_button = tk.Button(window, text="Greet Me!", command=greet)
greet_button.pack()

# Create labels to display greeting and birth year
let greeting_label = tk.Label(window, text="")
greeting_label.pack()

let birth_label = tk.Label(window, text="")
birth_label.pack()

# Start the GUI loop
window.mainloop()

```

After writing it, compiled it to `.py` file.

Here is the other way to make HTML application with Anaconda.

Put this cond in Anaconda file.

```html
# Anaconda Web App Example: Simple Web Interaction

# Define the HTML template for the app
let html_template = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anaconda Web App</title>
    <script>
        function greet() {
            // Get user input
            let name = document.getElementById("name").value;
            let age = document.getElementById("age").value;

            // Calculate birth year
            let current_year = 2025;
            let birth_year = current_year - toInt(age);

            // Display greeting and birth year
            document.getElementById("greeting").innerText = "Hello, " + name + "!";
            document.getElementById("birth_year").innerText = "You were born in the year: " + birth_year;
        }
    </script>
</head>
<body>
    <h1>Welcome to the Anaconda Web App</h1>
    <p>Enter your name and age to get a greeting and your birth year!</p>

    <label for="name">Name:</label>
    <input type="text" id="name" name="name"><br><br>

    <label for="age">Age:</label>
    <input type="number" id="age" name="age"><br><br>

    <button onclick="greet()">Greet Me!</button>

    <h2 id="greeting"></h2>
    <h3 id="birth_year"></h3>
</body>
</html>
"""

# Write the HTML template to the output file
let output_file = "app.html"
let file = openFile(output_file, "w")
file.write(html_template)
file.close()

# Print success message
print "Web app has been successfully created and saved to " + output_file

```

Now compiled it to `.html` file
