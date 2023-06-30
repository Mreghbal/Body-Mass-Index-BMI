import tkinter as tk

def calculate_bmi():
    weight = float(weight_entry.get())
    height = float(height_entry.get())

    bmi = weight / (height ** 2)

    result_label.config(text="Your BMI is: {:.2f}".format(bmi))
    condition_label.config(text="Condition: {}".format(get_condition(bmi)))

def get_condition(bmi):
    if bmi < 18.5:
        return "Underweight"
    elif 18.5 <= bmi < 24.9:
        return "Normal weight"
    elif 24.9 <= bmi < 29.9:
        return "Overweight"
    else:
        return "Obese"

# Create the main window
window = tk.Tk()
window.title("BMI Calculator")

# Create input labels and entry fields
weight_label = tk.Label(window, text="Weight (kg):")
weight_label.pack()
weight_entry = tk.Entry(window)
weight_entry.pack()

height_label = tk.Label(window, text="Height (m):")
height_label.pack()
height_entry = tk.Entry(window)
height_entry.pack()

# Create a button to calculate BMI
calculate_button = tk.Button(window, text="Calculate", command=calculate_bmi)
calculate_button.pack()

# Create labels to display the result
result_label = tk.Label(window, text="")
result_label.pack()

condition_label = tk.Label(window, text="")
condition_label.pack()

# Start the main event loop
window.mainloop()
