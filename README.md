# salary-tracker


A Python project that models employees and their salary levels using object-oriented programming. Each Employee has a name, a level, and a salary that is set automatically from the level. Promotions are validated so an employee can only move up, never down.

Note: This is a freeCodeCamp lab project. I completed it with guidance and assistance while learning Python.

Features

	•	Employee class with name, level, and salary attributes
	•	Base salaries stored per level (trainee, junior, mid-level, senior)
	•	Salary updates automatically when the level changes
	•	Input validation using property setters:
	•	name and level must be strings
	•	level must be one of the valid levels
	•	Setting the same level again is rejected
	•	Demotion to a lower level is rejected
	•	Friendly __str__ and developer-friendly __repr__ methods
	•	Confirmation messages when a name is updated or an employee is promoted

Concepts Practiced

	•	Classes and objects
	•	Class attributes (shared base salary table)
	•	@property getters and setters (encapsulation)
	•	Raising TypeError and ValueError for bad input
	•	__str__ and __repr__
	•	isinstance() and hasattr()

Getting Started

Prerequisites

	•	Python 3.8 or higher

Run it

git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
python salary_tracker.py

Example Usage

emp = Employee("David", "junior")

print(emp)         # David: junior
print(repr(emp))   # Employee('David', 'junior')

emp.name = "Dave"      # 'name' updated to 'Dave'.
emp.level = "senior"   # 'Dave' promoted to 'senior'.

emp.level = "trainee"  # ValueError: Cannot change to lower level.
emp.name = 123         # TypeError: 'name' must be a string.



What I Learned

	•	How to protect object data with properties and validation
	•	How to give clear error messages with the right exception types
	•	How a class-level dictionary can drive instance behavior

Acknowledgements

Built as part of the freeCodeCamp Python curriculum. I received assistance while working through this lab.

