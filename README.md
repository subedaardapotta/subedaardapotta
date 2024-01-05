def calculate_bmi(weight_kg, age):
    if weight_kg <= 0 or age <= 0:
        return "Invalid input. Weight and age must be positive values."

    # BMI formula using weight and age (for the sake of example)
    bmi = weight_kg / (age * age)

    return bmi

def categorize_fitness(bmi):
    if 18.5 <= bmi <= 24.9:
        return "Fit"
    else:
        return "Unfit"

# Input
weight = float(input("Enter weight in kilograms: "))
age = int(input("Enter age in years: "))

# Calculate BMI
result_bmi = calculate_bmi(weight, age)
print(f"Body Mass Index (BMI): {result_bmi}")

# Categorize fitness
fitness_category = categorize_fitness(result_bmi)
print(f"You are {fitness_category}.")
 
