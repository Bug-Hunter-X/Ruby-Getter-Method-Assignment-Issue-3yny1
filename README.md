# Ruby Getter Method Assignment

This repository demonstrates a common pitfall in Ruby regarding the assignment of values to methods that act as getters.  Unlike some other languages where such assignment modifies the object's state, in Ruby this does not work as expected.

The `bug.rb` file shows the incorrect approach, and `bugSolution.rb` provides the proper solution.

## How to run the code
1. Clone the repository.
2. Navigate to the repository's directory.
3. Run `ruby bug.rb` and `ruby bugSolution.rb` using your Ruby interpreter.

## Problem and Solution
The problem lies in attempting to directly assign a new value via the `value` method, which is designed only to return the current value. The solution is to use an appropriate setter method (or directly update the instance variable).