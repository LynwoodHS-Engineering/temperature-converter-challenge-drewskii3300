## Python Function Challenge: Temperature Converter

Your task is to create a temperature conversion program using Python functions. This program will allow users to convert temperatures between Celsius and Fahrenheit scales.

**Requirements:**

1. Create two functions:
   - `celsius_to_fahrenheit(celsius)`: Converts Celsius to Fahrenheit
   - `fahrenheit_to_celsius(fahrenheit)`: Converts Fahrenheit to Celsius

2. Implement a main menu function that displays options and returns the user's choice.

3. Use a while loop to keep the program running until the user chooses to quit.

**Function Formulas:**
- Celsius to Fahrenheit: $$F = (C \times 9/5) + 32$$
- Fahrenheit to Celsius: $$C = (F - 32) \times 5/9$$

**Program Structure:**

def celsius_to_fahrenheit(celsius):
    """Converts Celsius to Fahrenheit.""" 
    return (celsius * 9/5) + 32 
    
def fahrenheit_to_celsius(fahrenheit):
       """Converts Fahrenheit to Celsius.""" 
       return (fahrenheit - 32) * 5/9 
       
def menu():
    """Displays the menu and returns the user's choice.""" 
    print("\nTemperature Converter") 
    print("1. Celsius to Fahrenheit") 
    print("2. Fahrenheit to Celsius") 
    print("3. Exit")
    return input("Choose an option (1-3): ") 
    
def main(): 
    """Main function to run the program.""" 
    while True: 
        choice = menu() 
        if choice == '1': 
        celsius = float(input("Enter temperature in Celsius: ")) 
        print(f"{celsius}°C is {celsius_to_fahrenheit(celsius):.2f}°F") 
        elif choice == '2': 
             fahrenheit = float(input("Enter temperature in Fahrenheit: ")) 
             print(f"{fahrenheit}°F is {fahrenheit_to_celsius(fahrenheit):.2f}°C") 
        elif choice == '3': 
             print("Goodbye!") 
             break 
         else: 
            print("Invalid choice. Please enter 1, 2, or 3.") 
# Run the program 
main()


**Bonus Challenge:**
Add a third conversion option for Kelvin, including functions to convert to and from Kelvin.

## Submission:  Submit your code here and click "mark as done" on Google Classroom.
