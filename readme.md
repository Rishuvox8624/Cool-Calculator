# Cool Calculator (Demo Repository)

*An example repository to demonstrate collaboration on projects with GitHub
pull requests.*

## The Cool Calculator

This calculator aims to implement a python-based compiler for a Scheme-like syntax for simple arithmetic operations. This Scheme-like syntax uses
parentheses and prefix notation to indicate functional operations. For example:

| Operation | Python Syntax | Scheme-like Syntax |
| --- | --- | --- |
| addition | `a + b` | `(+ a b)` |
| subtraction  | `a - b` | `(- a b)` |
| multiplication | `a * b` | `(* a b)` |
| division | `a / b` | `(/ a b)` |

Further, operations can be nested as follows:

| Python Syntax | Scheme-like Syntax |
| --- | --- |
| `(a + b) * c` |  `(* (+ a b) c)` |

## Making Your Contribution

I have already implemented the addition operation, and it is up to you to
implement one of the other operations and contribute to this project.
Here's how:

1. First fork this repository to your own GitHub account online.
2. Clone that forked repository to your computer.
3. Create and check out a new branch for the operation you choose to implement.
4. Make edits to the `operations.py` file.

   ```python
   # SUBTRACTION Operation Entry ##############################
   # Desired Functionality: (- a b) = {{1. YOUR OPERATION IMPLEMENTATION}}

   def subtract(a, b):
	     return {{2. YOUR OPERATION IMPLEMENTATION}}

   sym_dict['-'] = ('{{3. IMPLEMENTATION FUNCTION}}', '{{4. YOUR NAME}}')
   ############################################################
   ```

   1. Add comments to indicate how your implementation works.
   2. Add the implementation in the return statement
   3. Add the implementation function name (e.g. subtract).
   4. Add your name as the author.

5. Commit those edits and push them back up to your GitHub repository.
7. Create a Pull Request to merge these changes into the original repository.

__See [Exercise 2](https://github.com/CorbanSwain/Git-Tutorial/blob/master/exercises/exercise_2.md)
in my [Git and GitHub Tutorial](https://github.com/CorbanSwain/Git-Tutorial)
for more information.__


## The End Result

*When you think your implementation is working take the following steps to test
it*

1. Navigate to the repository folder and start up a python3 console.
1. Type the following at the python prompt:
   ```python
   from calculator import compute
   ```
1. To test the addition operation (already implemented) type:
   ```python
   compute('(+ 1 3)')
   ```
   You should then see:
   ```python
   >>> compute('(+ 1 3)')
   Thanks for the "+" function, Corban S.!
   (+ 1 3) = 4
   ```
1. Now test your own implementation and nested implementations (as demonstrated
   in the second table above).
