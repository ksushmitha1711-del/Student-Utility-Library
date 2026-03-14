# Contributing Guide

Thank you for your interest in contributing to the Student Utility Library! This guide will help you get started with making your first contribution.

## 🎯 How to Contribute
# Introduction

Thank you for your interest in contributing to the Student Utility Library. This guide explains the steps required to implement functions and contribute effectively to the project.

1. Choosing a Function

Search the source code for functions marked with:
# TODO: Implement this function
Begin with simple functions and then move to more advanced implementations.

2. Recommended Order for Implementation
Beginner Level

Start with basic functions.
String Utilities
reverse_string()
count_words()
capitalize_words()
Math Utilities
factorial()
is_prime()
mean()
Intermediate Level
String Utilities
is_palindrome()
count_characters()
is_anagram()
Math Utilities
gcd()
lcm()
fibonacci()
median()
File Utilities
read_file()
write_file()
count_lines()
Advanced Level
Data Structures
Stack
Queue
LinkedList
Algorithms
Sorting algorithms
Searching algorithms
File Handling
CSV and JSON operations

# Implementation Process

Follow these steps when implementing a function:
Step 1: Read Documentation
Each function contains a docstring that explains:
Purpose of the function
Input parameters
Return values
Example usage

Step 2: Understand Test Cases
Review the corresponding test files inside the tests/ directory to understand expected behavior.

Step 3: Implement the Function
Replace the pass statement with your implementation.

Step 4: Run Specific Tests
python -m pytest tests/test_string_utils.py::TestStringUtils::test_reverse_string -v

Step 5: Run All Tests
python -m pytest tests/ -v

# Coding Standards

Follow these guidelines:

Follow PEP 8 coding style.

Use clear and meaningful variable names.

Include type hints for function parameters and return types.

Write docstrings for any new functions.

### Example Implementation

Here's how you might implement the `reverse_string` function:

```python
def reverse_string(text: str) -> str:
    """
    Reverse the given string.

    Args:
        text (str): Input string

    Returns:
        str: Reversed string
    """
    return text[::-1]
    # Method 1: Using string slicing (most Pythonic)
    return text[::-1]
    
    # Alternative methods:
    # Method 2: Using reversed() and join()
    # return ''.join(reversed(text))
    
    # Method 3: Using a loop
    # result = ""
    # for char in text:
    #     result = char + result
    # return result
```

### Testing Your Implementation

After implementing `reverse_string`, you can test it:

```python
# Run the specific test
from src.string_utils import reverse_string

print(reverse_string("hello"))

#out put 
olleh

# Bug Reporting

If a bug is discovered:

Create an issue describing the problem.

Submit a fix using a pull request.

Include test cases demonstrating the issue.

## 🏆 Recognition
Contributors will be recognized in several ways:

1. **README Contributors Section**: Your name will be added to the contributors list
2. **Git History**: Your commits will be part of the project history
3. **Learning Portfolio**: Use this contribution in your programming portfolio


# Best Practices
For Beginners

Start with simple functions.

Carefully read the docstring.

Check test cases for expected results.

Use debugging techniques such as print statements.

Common Mistakes to Avoid

Ignoring edge cases (empty strings, negative numbers).

Changing the function signature.

Not testing the code before submission.

## 📚 Learning Resources

- **Python Basics**: [Python.org Tutorial](https://docs.python.org/3/tutorial/)
- **Style Guide**: [PEP 8](https://pep8.org/)
- **Type Hints**: [Python Type Hints](https://docs.python.org/3/library/typing.html)
- **Testing**: [pytest Documentation](https://docs.pytest.org/)
- **Algorithms**: [Algorithm Visualizations](https://visualgo.net/)

## 🤝 Getting Help

If you're stuck:

1. Read the function's docstring again
2. Look at the test cases for examples
3. Check the hints in the TODO comments
4. Ask for help in project discussions
5. Look up similar functions online for inspiration

## 🎉 Making Your First Contribution

1. Pick a simple function like `reverse_string()`
2. Read its docstring and understand what it should do
3. Look at the test cases in `tests/test_string_utils.py`
4. Implement the function
5. Run the tests to make sure it works
6. Celebrate your contribution! 🎊

Remember: Every expert was once a beginner. Don't be afraid to start small and learn as you go!

---

Happy coding! 🚀