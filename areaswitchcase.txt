#include <stdio.h>

void main() {
    int choice;
    float area, perimeter;
    
    printf("1. Calculate the area of a circle\n");
    printf("2. Calculate the area of a rectangle\n");
    printf("3. Calculate the area of a square\n");
    printf("4. Quit\n");
    printf("Enter your choice (1/2/3/4): ");
    scanf("%d", &choice);
    
    switch (choice) {
        case 1: // Calculate the area and perimeter of a circle
            {
                float radius;
                printf("Enter the radius of the circle: ");
                scanf("%f", &radius);
                area = 3.14159 * radius * radius;
                perimeter = 2 * 3.14159 * radius;
                printf("The area of the circle is: %f\n", area);
                printf("The perimeter of the circle is: %f\n", perimeter);
            }
            break;
        case 2: // Calculate the area and perimeter of a rectangle
            {
                float length, breadth; // Changed "width" to "breadth"
                printf("Enter the length of the rectangle: ");
                scanf("%f", &length);
                printf("Enter the breadth of the rectangle: "); // Changed "width" to "breadth"
                scanf("%f", &breadth); // Changed "width" to "breadth"
                area = length * breadth; // Changed "width" to "breadth"
                perimeter = 2 * (length + breadth); // Changed "width" to "breadth"
                printf("The area of the rectangle is: %f\n", area);
                printf("The perimeter of the rectangle is: %f\n", perimeter);
            }
            break;
        case 3: // Calculate the area and perimeter of a square
            {
                float side;
                printf("Enter the side of the square: ");
                scanf("%f", &side);
                area = side * side;
                perimeter = 4 * side;
                printf("The area of the square is: %f\n", area);
                printf("The perimeter of the square is: %f\n", perimeter);
            }
            break;
        case 4: // Quit the program
            printf("Exiting the program. Goodbye!\n");
            break;
        default: // Invalid choice
            printf("Invalid choice. Please enter a valid option (1/2/3/4).\n");
    }
    
    
}

