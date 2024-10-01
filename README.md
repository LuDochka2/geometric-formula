# geometric-formulaimport math

def circle_area(radius):
    return math.pi * radius ** 2

def rectangle_area(length, width):
    return length * width

def triangle_area(base, height):
    return 0.5 * base * height

# Main function to select the shape and compute the area
def main():
    print("Choose a shape to calculate the area:")
    print("1. Circle")
    print("2. Rectangle")
    print("3. Triangle")
    
    choice = input("Enter the number corresponding to the shape: ")

    if choice == '1':
        radius = float(input("Enter the radius of the circle: "))
        area = circle_area(radius)
        print(f"The area of the circle is: {area:.2f} square units.")
        
    elif choice == '2':
        length = float(input("Enter the length of the rectangle: "))
        width = float(input("Enter the width of the rectangle: "))
        area = rectangle_area(length, width)
        print(f"The area of the rectangle is: {area:.2f} square units.")
        
    elif choice == '3':
        base = float(input("Enter the base of the triangle: "))
        height = float(input("Enter the height of the triangle: "))
        area = triangle_area(base, height)
        print(f"The area of the triangle is: {area:.2f} square units.")
        
    else:
        print("Invalid choice. Please choose a valid shape.")

# Run the main function
if __name__ == "__main__":
    main()
