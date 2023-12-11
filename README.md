Shape Calculator
This project implements a shape calculator for rectangles and squares, emphasizing object-oriented programming principles. The Rectangle class is designed to handle rectangles, and the Square class is a specialized subclass of Rectangle. The main functionalities and usage examples are outlined below.

Rectangle Class
Methods
__init__(self, width, height): Initializes the Rectangle with the specified width and height.
set_width(self, width): Sets the width of the Rectangle.
set_height(self, height): Sets the height of the Rectangle.
get_area(self): Returns the area of the Rectangle (width * height).
get_perimeter(self): Returns the perimeter of the Rectangle (2 * width + 2 * height).
get_diagonal(self): Returns the diagonal of the Rectangle ((width ** 2 + height ** 2) ** .5).
get_picture(self): Returns a string representation of the Rectangle using lines of "*". If width or height is larger than 50, returns "Too big for picture.".
get_amount_inside(self, shape): Takes another shape (square or rectangle) as an argument. Returns the number of times the passed-in shape could fit inside the Rectangle (with no rotations).
Example
python
Copy code
rect = shape_calculator.Rectangle(10, 5)
print(rect.get_area())
rect.set_height(3)
print(rect.get_perimeter())
print(rect)
print(rect.get_picture())

sq = shape_calculator.Square(9)
print(sq.get_area())
sq.set_side(4)
print(sq.get_diagonal())
print(sq)
print(sq.get_picture())

rect.set_height(8)
rect.set_width(16)
print(rect.get_amount_inside(sq))
Square Class
The Square class is a subclass of Rectangle and inherits its methods.

Additional Method
set_side(self, side): Sets the side length of the Square, adjusting both width and height.
Example
python
Copy code
sq = shape_calculator.Square(9)
print(sq.get_area())
sq.set_side(4)
print(sq.get_diagonal())
print(sq)
print(sq.get_picture())
Development
Write your code in shape_calculator.py. For development, you can use main.py to test your shape_calculator() function. Click the "run" button, and main.py will execute.

Testing
Unit tests are available in test_module.py. They will run automatically whenever you hit the "run" button. Ensure that your implementations pass all tests before finalizing your project.
