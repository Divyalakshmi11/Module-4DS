# Exp.No:17  
## EXCEPTION HANDLING

---

### AIM  
To create a Python program that prompts the user for a list of grades separated by commas, splits the string into individual grades, and uses exception handling to inform the user if the values they entered cannot be converted to integers.

---

### ALGORITHM

1. Begin the program.  
2. Read a string `input_str` from the user using `input()`.  
3. Split the input string using commas (`,`) to create a list of grades.  
4. Use a `try` block to attempt converting each item in the grades list to an integer and store the result in `l1`.  
5. If the conversion is successful, print the list `l1` containing the integer values.  
6. If an error occurs during conversion (for example, if the input is not a valid number), catch the exception and print an error message: `"The grades you entered were in an invalid format."` along with the original grades list.  
7. Terminate the program.

---

### PROGRAM

```
def process_grades():
   
    grades_input = input()
    grades_list = grades_input.split(",")

    try:
        grades_int = [int(grade.strip()) for grade in grades_list]
        return grades_int
    except ValueError:
        return f"The grades you entered were in an invalid format.\n{grades_list}"


result = process_grades()
print(result)



```

### OUTPUT
<img width="1017" height="201" alt="image" src="https://github.com/user-attachments/assets/4a6e3b68-b892-4e10-ba84-634a5477ef0d" />


### RESULT
Therefore, the output is the example to create a Python program that prompts the user for a list of grades separated by commas, splits the string into individual grades, and uses exception handling to inform the user if the values they entered cannot be converted to integers.
