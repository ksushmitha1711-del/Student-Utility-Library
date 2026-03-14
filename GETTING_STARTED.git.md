# Getting Started Guide

# Introduction

Welcome to the Student Utility Library project. This guide provides step-by-step instructions to help you set up the project environment and make your first contribution by implementing utility functions

## 📋 Quick Setup

Follow these steps to configure the project on your system.

Step 1: Install Python
Ensure Python 3.8 or later is installed on your system.
You can verify using:
</>Bash 
python --version

Step 2: Install Project Dependencies
Install the required libraries listed in requirements.txt.
</>Bash 
pip install -r requirements.txt

Step 3: Verify Installation
Run the project test suite to confirm that the setup is working.
</>Bash 
python -m pytest tests/ -v

Note: Some tests will fail initially because the functions are not implemented yet. This is expected.

Step 4: Run Example Programs
You can explore the example usage of the project by running:
</>Bash
python examples/basic_usage.py

# Your First Contribution

To begin contributing, start by implementing a simple function.

Step 1: Select a Simple Function
Open the file:
src/string_utils/__init__.py
Find the following function:
def reverse_string(text: str) -> str:
    """
    Reverse the given string.

    TODO: Implement this function
    Hint: Use string slicing [::-1] or a loop
    """
    pass

Step 2: Implement the Function
Replace the pass statement with the implementation.
def reverse_string(text: str) -> str:
    """Reverse the given string."""
    return text[::-1]

 Step 3: Test the Function
Run the specific test for this function.
python -m pytest tests/test_string_utils.py::TestStringUtils::test_reverse_string -v

step 4: Successful Contribution

If the test passes, your implementation is correct. 🎉
You have successfully made your first contribution.

## 📂 Project Structure Overview

```
StudentUtilityLibrary/
├── src/                    # Main source code
│   ├── string_utils/       # String manipulation functions
│   ├── math_utils/         # Mathematical calculations  
│   ├── data_structures/    # Stack, Queue, LinkedList, etc.
│   ├── algorithms/         # Sorting, searching algorithms
│   └── file_utils/         # File operations
├── tests/                  # Unit tests for all modules
├── examples/               # Usage examples and demos
├── README.md               # Project overview
├── CONTRIBUTING.md         # Detailed contribution guide
└── requirements.txt        # Project dependencies
```

## 🚀 Recommended Learning Path

### Beginner Level (Start Here!)
1. String utilities: `reverse_string`, `count_words`, `capitalize_words`
2. Math utilities: `factorial`, `is_prime`, `mean`
3. File utilities: `read_file`, `write_file`

### Intermediate Level
1. String utilities: `is_palindrome`, `is_anagram`  
2. Math utilities: `gcd`, `lcm`, `fibonacci`
3. Simple algorithms: `linear_search`, `bubble_sort`

### Advanced Level
1. Data structures: `Stack`, `Queue`, `LinkedList`, `BinaryTree`
2. Advanced algorithms: `merge_sort`, `quick_sort`, `binary_search`
3. Complex file operations: CSV/JSON handling

## 🔧 Available Commands

### Testing
```bash
# Run all tests
python -m pytest tests/ -v

# Run tests for specific module
python -m pytest tests/test_string_utils.py -v

# Run specific test
python -m pytest tests/test_string_utils.py::TestStringUtils::test_reverse_string -v

# Run tests with coverage
python -m pytest tests/ --cov=src --cov-report=html
```

### Code Quality
```bash
# Format code with black
python -m black src/ tests/ examples/

# Type checking with mypy
python -m mypy src/

# Linting with flake8
python -m flake8 src/ tests/ examples/
```

### Examples
```bash
# Run main usage examples
python examples/basic_usage.py

# Import and test individual functions
python -c "from src.string_utils import reverse_string; print(reverse_string('hello'))"
```

## 💡 Tips for Success

### Understanding Function Requirements
1. **Read the docstring carefully** - it explains exactly what the function should do
2. **Check the examples** - they show expected input/output
3. **Look at the test cases** - they define the exact behavior expected
4. **Pay attention to type hints** - they specify parameter and return types

### Debugging Your Code
1. **Use print statements** to see what your code is doing
2. **Test with simple inputs first** before trying complex cases
3. **Run the specific test** for your function to see detailed error messages
4. **Check edge cases** like empty strings, zero values, etc.

### Common Mistakes to Avoid
- Not handling edge cases (empty inputs, negative numbers)
- Not following the exact function signature
- Implementing different behavior than described in docstring
- Not testing code before considering it complete

## 🏆 Recognition System

Your contributions are recognized through:
- **Git commit history** - permanent record of your work
- **Test passes** - green checkmarks showing working code  
- **Code reviews** - feedback to help you improve
- **Portfolio material** - real open-source contributions for your resume

## 🤝 Getting Help

### If You're Stuck:
1. Re-read the function's docstring and examples
2. Look at the test cases for that function
3. Search online for similar problems and solutions
4. Ask questions in project discussions
5. Start with an even simpler function and build up

### Online Resources:
- [Python.org Tutorial](https://docs.python.org/3/tutorial/)
- [Real Python](https://realpython.com/) - excellent Python tutorials
- [Stack Overflow](https://stackoverflow.com/) - programming Q&A
- [LeetCode](https://leetcode.com/) - algorithm practice problems

## 🎊 Ready to Start?

1. Pick a function from the beginner list
2. Open the file and find the function
3. Read the docstring and understand what it should do
4. Replace `pass` with your implementation
5. Test it and fix any issues
6. Move on to the next function!

Remember: Every expert was once a beginner. The goal is learning, not perfection!

**Happy coding!** 🚀