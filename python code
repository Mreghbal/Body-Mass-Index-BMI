def calculate_bmi(weight, height):
    bmi = weight / (height ** 2)
    return bmi

def get_condition(bmi):
    if bmi < 18.5:
        return "Underweight"
    elif 18.5 <= bmi < 24.9:
        return "Normal weight"
    elif 24.9 <= bmi < 29.9:
        return "Overweight"
    else:
        return "Obese"

def main():
    weight = float(input("Enter your weight in kilograms: "))
    height = float(input("Enter your height in meters: "))

    bmi = calculate_bmi(weight, height)

    print("Your BMI is:", round(bmi, 2))
    print("Condition:", get_condition(bmi))

if __name__ == "__main__": 
    main()
