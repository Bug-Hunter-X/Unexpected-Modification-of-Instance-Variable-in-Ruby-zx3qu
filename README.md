# Unexpected Instance Variable Modification

This repository demonstrates a potential issue in Ruby related to directly modifying instance variables outside of defined methods.  While functional, this practice breaks encapsulation, leading to maintainability and debugging challenges.  The `bug.rb` file showcases the issue, while `bugSolution.rb` presents a more robust approach.

The problem arises when you bypass accessor methods and manipulate instance variables directly using methods like `instance_variable_set` or `instance_variable_get`. This can lead to unforeseen consequences, especially in larger projects where changes might introduce subtle bugs.

The solution encourages using accessor methods (`attr_accessor`, `attr_reader`, `attr_writer`) to maintain data integrity and improve code clarity and maintainability.