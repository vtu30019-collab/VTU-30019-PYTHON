# Initialize the list of grades
grades = [85, 90, 78, 92, 88]

# Display the grades list
print("Grades List:", grades)

# Prompt the user to enter the index of the grade they want to view
try:
    index = int(input("Enter the index of the grade you want to view: "))
    # Attempt to display the grade at the specified index
    print(f"The grade at index {index} is: {grades[index]}")
except IndexError:
    # Handle the case where the index is out of range
    print("Invalid index. Please enter a valid index.")
except ValueError:
    # Handle the case where the input is not an integer
    print("Invalid input. Please enter a numerical index.")
