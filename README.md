# Patterns

def print_pattern(shape, size):
    if shape == "square":
        for i in range(size):
            print("* " * size)
    elif shape == "rectangle":
        width = int(input("Enter the width of the rectangle: "))
        for i in range(size):
            print("* " * width)
    elif shape == "triangle":
        for i in range(1, size + 1):
            print(" " * (size - i) + "* " * i)
    else:
        print("Invalid shape. Please enter 'square', 'rectangle', or 'triangle'.")

shape = input("Enter the shape (square, rectangle, triangle): ")
size = int(input("Enter the size of the shape: "))

print_pattern(shape, size)
