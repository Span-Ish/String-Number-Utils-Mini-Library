# my_utils

A simple Python utility library built for learning Test-Driven Development (TDD), unit testing with pytest, and code coverage analysis.

---

## Project Structure

my_utils/
my_utils/
__init__.py
string_utils.py
number_utils.py

tests/
test_string_utils.py
test_number_utils.py

pytest.ini
requirements.txt
venv/

---

## Features

### String Utilities

- truncate(text, max_len)
  → Truncates text and adds "..." if needed

- title_case(text)
  → Converts text to title case

- is_palindrome(text)
  → Checks if text is a palindrome (ignores spaces and case)

- count_vowels(text)
  → Counts number of vowels in a string

---

### Number Utilities

- clamp(value, min_val, max_val)
  → Clamps a number within a range

- is_prime(n)
  → Returns True if number is prime

- fibonacci(n)
  → Returns the nth Fibonacci number

- percentage(part, whole)
  → Returns percentage value

---

## Setup

Install dependencies:

pip install -r requirements.txt

Or manually:

pip install pytest pytest-cov

---

## Running Tests

Run all tests:

python -m pytest

---

## Code Coverage

Run tests with coverage:

python -m pytest --cov=my_utils --cov-report=term-missing

Goal: at least 95% coverage

---

## Example Usage

from my_utils.string_utils import truncate, is_palindrome
from my_utils.number_utils import fibonacci, percentage

print(truncate("hello world", 8))
print(is_palindrome("racecar"))
print(fibonacci(10))
print(percentage(25, 100))

---

## Notes

- Always run commands from the project root
- Do not run files inside the my_utils folder directly
- Use python -m pytest if pytest command does not work on Windows
