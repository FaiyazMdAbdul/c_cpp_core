# C and C++ Programming Basics Guide

## Table of Contents
- [C Programming Basics](#c-programming-basics)
- [C++ Programming Basics](#c-programming-basics-1)

---

# C Programming Basics

## 1. Hello World Program

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

## 2. Data Types

### Basic Data Types
```c
#include <stdio.h>

int main() {
    // Integer types
    int age = 25;
    short small_num = 100;
    long big_num = 1000000L;
    
    // Character type
    char grade = 'A';
    
    // Floating point types
    float price = 19.99f;
    double precise_value = 3.14159265359;
    
    // Boolean (C99 and later)
    #include <stdbool.h>
    bool is_valid = true;
    
    printf("Age: %d\n", age);
    printf("Grade: %c\n", grade);
    printf("Price: %.2f\n", price);
    printf("Precise: %.10lf\n", precise_value);
    
    return 0;
}
```

## 3. Variables and Constants

```c
#include <stdio.h>
#define PI 3.14159  // Macro constant

int main() {
    // Variables
    int x = 10;
    int y = 20;
    
    // Constants
    const int MAX_SIZE = 100;
    
    printf("x = %d, y = %d\n", x, y);
    printf("PI = %.5f\n", PI);
    printf("MAX_SIZE = %d\n", MAX_SIZE);
    
    return 0;
}
```

## 4. Operators

```c
#include <stdio.h>

int main() {
    int a = 10, b = 3;
    
    // Arithmetic operators
    printf("a + b = %d\n", a + b);
    printf("a - b = %d\n", a - b);
    printf("a * b = %d\n", a * b);
    printf("a / b = %d\n", a / b);
    printf("a %% b = %d\n", a % b);
    
    // Comparison operators
    printf("a == b: %d\n", a == b);
    printf("a != b: %d\n", a != b);
    printf("a > b: %d\n", a > b);
    printf("a < b: %d\n", a < b);
    
    // Logical operators
    int x = 1, y = 0;
    printf("x && y: %d\n", x && y);
    printf("x || y: %d\n", x || y);
    printf("!x: %d\n", !x);
    
    // Increment/Decrement
    printf("a++: %d\n", a++);  // Post-increment
    printf("++a: %d\n", ++a);  // Pre-increment
    
    return 0;
}
```

## 5. Control Structures

### If-Else Statement
```c
#include <stdio.h>

int main() {
    int score = 85;
    
    if (score >= 90) {
        printf("Grade: A\n");
    } else if (score >= 80) {
        printf("Grade: B\n");
    } else if (score >= 70) {
        printf("Grade: C\n");
    } else {
        printf("Grade: F\n");
    }
    
    return 0;
}
```

### Switch Statement
```c
#include <stdio.h>

int main() {
    char operator = '+';
    int a = 10, b = 5;
    
    switch (operator) {
        case '+':
            printf("%d + %d = %d\n", a, b, a + b);
            break;
        case '-':
            printf("%d - %d = %d\n", a, b, a - b);
            break;
        case '*':
            printf("%d * %d = %d\n", a, b, a * b);
            break;
        case '/':
            if (b != 0)
                printf("%d / %d = %d\n", a, b, a / b);
            else
                printf("Division by zero!\n");
            break;
        default:
            printf("Invalid operator\n");
    }
    
    return 0;
}
```

## 6. Loops

### For Loop
```c
#include <stdio.h>

int main() {
    // Simple for loop
    for (int i = 1; i <= 5; i++) {
        printf("Count: %d\n", i);
    }
    
    // Nested for loop - multiplication table
    for (int i = 1; i <= 3; i++) {
        for (int j = 1; j <= 3; j++) {
            printf("%d x %d = %d\t", i, j, i * j);
        }
        printf("\n");
    }
    
    return 0;
}
```

### While Loop
```c
#include <stdio.h>

int main() {
    int i = 1;
    
    while (i <= 5) {
        printf("While loop: %d\n", i);
        i++;
    }
    
    return 0;
}
```

### Do-While Loop
```c
#include <stdio.h>

int main() {
    int i = 1;
    
    do {
        printf("Do-while loop: %d\n", i);
        i++;
    } while (i <= 5);
    
    return 0;
}
```

## 7. Arrays

```c
#include <stdio.h>

int main() {
    // Array declaration and initialization
    int numbers[5] = {1, 2, 3, 4, 5};
    char name[] = "Hello";
    
    // Accessing array elements
    printf("First element: %d\n", numbers[0]);
    printf("Third element: %d\n", numbers[2]);
    
    // Array traversal
    printf("Array elements: ");
    for (int i = 0; i < 5; i++) {
        printf("%d ", numbers[i]);
    }
    printf("\n");
    
    // String (character array)
    printf("String: %s\n", name);
    
    // 2D Array
    int matrix[2][3] = {{1, 2, 3}, {4, 5, 6}};
    
    printf("2D Array:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++) {
            printf("%d ", matrix[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
```

## 8. Functions

```c
#include <stdio.h>

// Function declaration
int add(int a, int b);
void greet(char name[]);
int factorial(int n);

int main() {
    int result = add(5, 3);
    printf("5 + 3 = %d\n", result);
    
    greet("Alice");
    
    printf("Factorial of 5: %d\n", factorial(5));
    
    return 0;
}

// Function definition
int add(int a, int b) {
    return a + b;
}

void greet(char name[]) {
    printf("Hello, %s!\n", name);
}

int factorial(int n) {
    if (n <= 1)
        return 1;
    else
        return n * factorial(n - 1);
}
```

## 9. Pointers

```c
#include <stdio.h>

void swap(int *a, int *b);

int main() {
    int x = 10;
    int *ptr = &x;  // Pointer declaration
    
    printf("Value of x: %d\n", x);
    printf("Address of x: %p\n", &x);
    printf("Value of ptr: %p\n", ptr);
    printf("Value pointed by ptr: %d\n", *ptr);
    
    // Pointer arithmetic
    int arr[] = {1, 2, 3, 4, 5};
    int *p = arr;
    
    printf("Array elements using pointer:\n");
    for (int i = 0; i < 5; i++) {
        printf("%d ", *(p + i));
    }
    printf("\n");
    
    // Function with pointers
    int a = 5, b = 10;
    printf("Before swap: a = %d, b = %d\n", a, b);
    swap(&a, &b);
    printf("After swap: a = %d, b = %d\n", a, b);
    
    return 0;
}

void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
```

## 10. Structures

```c
#include <stdio.h>
#include <string.h>

// Structure definition
struct Student {
    int id;
    char name[50];
    float grade;
};

int main() {
    // Structure variable declaration
    struct Student student1;
    
    // Assigning values
    student1.id = 101;
    strcpy(student1.name, "John Doe");
    student1.grade = 85.5;
    
    // Structure initialization
    struct Student student2 = {102, "Jane Smith", 92.0};
    
    printf("Student 1:\n");
    printf("ID: %d\n", student1.id);
    printf("Name: %s\n", student1.name);
    printf("Grade: %.2f\n", student1.grade);
    
    printf("\nStudent 2:\n");
    printf("ID: %d, Name: %s, Grade: %.2f\n", 
           student2.id, student2.name, student2.grade);
    
    // Array of structures
    struct Student students[2] = {
        {103, "Alice", 88.0},
        {104, "Bob", 76.5}
    };
    
    printf("\nAll students:\n");
    for (int i = 0; i < 2; i++) {
        printf("%d: %s - %.2f\n", 
               students[i].id, students[i].name, students[i].grade);
    }
    
    return 0;
}
```

## 11. Dynamic Memory Allocation

```c
#include <stdio.h>
#include <stdlib.h>

int main() {
    int n;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    // Dynamic memory allocation
    int *ptr = (int*)malloc(n * sizeof(int));
    
    if (ptr == NULL) {
        printf("Memory allocation failed!\n");
        return 1;
    }
    
    // Input elements
    printf("Enter %d elements: ", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &ptr[i]);
    }
    
    // Display elements
    printf("Elements: ");
    for (int i = 0; i < n; i++) {
        printf("%d ", ptr[i]);
    }
    printf("\n");
    
    // Free allocated memory
    free(ptr);
    
    return 0;
}
```

## 12. File Handling

```c
#include <stdio.h>

int main() {
    FILE *file;
    char text[100];
    
    // Writing to file
    file = fopen("sample.txt", "w");
    if (file == NULL) {
        printf("Error opening file for writing!\n");
        return 1;
    }
    
    fprintf(file, "Hello, World!\n");
    fprintf(file, "This is a sample file.\n");
    fclose(file);
    
    // Reading from file
    file = fopen("sample.txt", "r");
    if (file == NULL) {
        printf("Error opening file for reading!\n");
        return 1;
    }
    
    printf("File contents:\n");
    while (fgets(text, sizeof(text), file) != NULL) {
        printf("%s", text);
    }
    
    fclose(file);
    
    return 0;
}
```

---

# C++ Programming Basics

## 1. Hello World Program

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
```

## 2. Input/Output Operations

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string name;
    int age;
    
    cout << "Enter your name: ";
    getline(cin, name);  // For strings with spaces
    
    cout << "Enter your age: ";
    cin >> age;
    
    cout << "Hello, " << name << "! You are " << age << " years old." << endl;
    
    return 0;
}
```

## 3. Data Types and Variables

```cpp
#include <iostream>
using namespace std;

int main() {
    // Basic data types
    int number = 42;
    double pi = 3.14159;
    char grade = 'A';
    bool is_student = true;
    string name = "John Doe";
    
    // Auto keyword (C++11)
    auto x = 10;        // int
    auto y = 3.14;      // double
    auto z = "Hello";   // const char*
    
    cout << "Number: " << number << endl;
    cout << "Pi: " << pi << endl;
    cout << "Grade: " << grade << endl;
    cout << "Is student: " << boolalpha << is_student << endl;
    cout << "Name: " << name << endl;
    
    return 0;
}
```

## 4. References and Pointers

```cpp
#include <iostream>
using namespace std;

void swap_by_reference(int &a, int &b);
void swap_by_pointer(int *a, int *b);

int main() {
    int x = 10;
    int &ref = x;  // Reference
    int *ptr = &x; // Pointer
    
    cout << "Original x: " << x << endl;
    cout << "Reference ref: " << ref << endl;
    cout << "Pointer *ptr: " << *ptr << endl;
    
    // Modifying through reference
    ref = 20;
    cout << "After modifying ref, x = " << x << endl;
    
    // Function calls
    int a = 5, b = 10;
    cout << "Before swap: a = " << a << ", b = " << b << endl;
    
    swap_by_reference(a, b);
    cout << "After reference swap: a = " << a << ", b = " << b << endl;
    
    swap_by_pointer(&a, &b);
    cout << "After pointer swap: a = " << a << ", b = " << b << endl;
    
    return 0;
}

void swap_by_reference(int &a, int &b) {
    int temp = a;
    a = b;
    b = temp;
}

void swap_by_pointer(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
```

## 5. Classes and Objects

```cpp
#include <iostream>
#include <string>
using namespace std;

class Student {
private:
    int id;
    string name;
    double gpa;
    
public:
    // Constructor
    Student(int student_id, string student_name, double student_gpa) {
        id = student_id;
        name = student_name;
        gpa = student_gpa;
    }
    
    // Default constructor
    Student() {
        id = 0;
        name = "Unknown";
        gpa = 0.0;
    }
    
    // Getter methods
    int getId() const { return id; }
    string getName() const { return name; }
    double getGpa() const { return gpa; }
    
    // Setter methods
    void setId(int student_id) { id = student_id; }
    void setName(string student_name) { name = student_name; }
    void setGpa(double student_gpa) { gpa = student_gpa; }
    
    // Method to display student info
    void display() const {
        cout << "ID: " << id << ", Name: " << name << ", GPA: " << gpa << endl;
    }
};

int main() {
    // Creating objects
    Student student1(101, "Alice", 3.8);
    Student student2; // Default constructor
    
    student1.display();
    student2.display();
    
    // Using setter methods
    student2.setId(102);
    student2.setName("Bob");
    student2.setGpa(3.5);
    
    cout << "After setting values:" << endl;
    student2.display();
    
    return 0;
}
```

## 6. Constructor and Destructor

```cpp
#include <iostream>
#include <string>
using namespace std;

class Rectangle {
private:
    double length;
    double width;
    
public:
    // Parameterized constructor
    Rectangle(double l, double w) : length(l), width(w) {
        cout << "Rectangle created with length " << length 
             << " and width " << width << endl;
    }
    
    // Copy constructor
    Rectangle(const Rectangle &other) {
        length = other.length;
        width = other.width;
        cout << "Rectangle copied" << endl;
    }
    
    // Destructor
    ~Rectangle() {
        cout << "Rectangle destroyed" << endl;
    }
    
    double area() const {
        return length * width;
    }
    
    void display() const {
        cout << "Rectangle: " << length << " x " << width 
             << ", Area: " << area() << endl;
    }
};

int main() {
    Rectangle rect1(5.0, 3.0);
    rect1.display();
    
    Rectangle rect2 = rect1;  // Copy constructor called
    rect2.display();
    
    return 0;
} // Destructors called here
```

## 7. Inheritance

```cpp
#include <iostream>
#include <string>
using namespace std;

// Base class
class Animal {
protected:
    string name;
    int age;
    
public:
    Animal(string n, int a) : name(n), age(a) {
        cout << "Animal constructor called" << endl;
    }
    
    virtual void makeSound() const {
        cout << name << " makes a sound" << endl;
    }
    
    void displayInfo() const {
        cout << "Name: " << name << ", Age: " << age << endl;
    }
    
    virtual ~Animal() {
        cout << "Animal destructor called" << endl;
    }
};

// Derived class
class Dog : public Animal {
private:
    string breed;
    
public:
    Dog(string n, int a, string b) : Animal(n, a), breed(b) {
        cout << "Dog constructor called" << endl;
    }
    
    void makeSound() const override {
        cout << name << " barks: Woof! Woof!" << endl;
    }
    
    void displayBreed() const {
        cout << "Breed: " << breed << endl;
    }
    
    ~Dog() {
        cout << "Dog destructor called" << endl;
    }
};

int main() {
    Dog myDog("Buddy", 3, "Golden Retriever");
    
    myDog.displayInfo();
    myDog.displayBreed();
    myDog.makeSound();
    
    // Polymorphism
    Animal* animalPtr = &myDog;
    animalPtr->makeSound(); // Calls Dog's makeSound()
    
    return 0;
}
```

## 8. Function Overloading

```cpp
#include <iostream>
using namespace std;

class Calculator {
public:
    // Function overloading - same name, different parameters
    int add(int a, int b) {
        return a + b;
    }
    
    double add(double a, double b) {
        return a + b;
    }
    
    int add(int a, int b, int c) {
        return a + b + c;
    }
    
    string add(string a, string b) {
        return a + b;
    }
};

int main() {
    Calculator calc;
    
    cout << "Int addition: " << calc.add(5, 3) << endl;
    cout << "Double addition: " << calc.add(5.5, 3.2) << endl;
    cout << "Three int addition: " << calc.add(1, 2, 3) << endl;
    cout << "String concatenation: " << calc.add("Hello", " World") << endl;
    
    return 0;
}
```

## 9. Operator Overloading

```cpp
#include <iostream>
using namespace std;

class Complex {
private:
    double real;
    double imag;
    
public:
    Complex(double r = 0, double i = 0) : real(r), imag(i) {}
    
    // Operator overloading for +
    Complex operator+(const Complex& other) const {
        return Complex(real + other.real, imag + other.imag);
    }
    
    // Operator overloading for <<
    friend ostream& operator<<(ostream& out, const Complex& c) {
        out << c.real;
        if (c.imag >= 0) out << "+";
        out << c.imag << "i";
        return out;
    }
    
    // Operator overloading for ==
    bool operator==(const Complex& other) const {
        return (real == other.real) && (imag == other.imag);
    }
};

int main() {
    Complex c1(3, 4);
    Complex c2(1, 2);
    Complex c3 = c1 + c2;  // Uses overloaded + operator
    
    cout << "c1 = " << c1 << endl;
    cout << "c2 = " << c2 << endl;
    cout << "c3 = c1 + c2 = " << c3 << endl;
    
    if (c1 == c2) {
        cout << "c1 and c2 are equal" << endl;
    } else {
        cout << "c1 and c2 are not equal" << endl;
    }
    
    return 0;
}
```

## 10. Templates

```cpp
#include <iostream>
#include <vector>
using namespace std;

// Function template
template <typename T>
T getMax(T a, T b) {
    return (a > b) ? a : b;
}

// Class template
template <typename T>
class Stack {
private:
    vector<T> elements;
    
public:
    void push(const T& element) {
        elements.push_back(element);
    }
    
    void pop() {
        if (!elements.empty()) {
            elements.pop_back();
        }
    }
    
    T top() const {
        if (!elements.empty()) {
            return elements.back();
        }
        throw runtime_error("Stack is empty");
    }
    
    bool empty() const {
        return elements.empty();
    }
    
    size_t size() const {
        return elements.size();
    }
};

int main() {
    // Function template usage
    cout << "Max of 10 and 20: " << getMax(10, 20) << endl;
    cout << "Max of 3.5 and 2.1: " << getMax(3.5, 2.1) << endl;
    cout << "Max of 'a' and 'z': " << getMax('a', 'z') << endl;
    
    // Class template usage
    Stack<int> intStack;
    intStack.push(10);
    intStack.push(20);
    intStack.push(30);
    
    cout << "Int stack size: " << intStack.size() << endl;
    cout << "Top element: " << intStack.top() << endl;
    
    Stack<string> stringStack;
    stringStack.push("Hello");
    stringStack.push("World");
    
    cout << "String stack top: " << stringStack.top() << endl;
    
    return 0;
}
```

## 11. STL (Standard Template Library)

```cpp
#include <iostream>
#include <vector>
#include <map>
#include <string>
#include <algorithm>
using namespace std;

int main() {
    // Vector
    vector<int> numbers = {5, 2, 8, 1, 9};
    
    cout << "Original vector: ";
    for (int num : numbers) {
        cout << num << " ";
    }
    cout << endl;
    
    // Sorting
    sort(numbers.begin(), numbers.end());
    cout << "Sorted vector: ";
    for (int num : numbers) {
        cout << num << " ";
    }
    cout << endl;
    
    // Adding elements
    numbers.push_back(15);
    cout << "After push_back(15): ";
    for (int num : numbers) {
        cout << num << " ";
    }
    cout << endl;
    
    // Map
    map<string, int> ages;
    ages["Alice"] = 25;
    ages["Bob"] = 30;
    ages["Charlie"] = 35;
    
    cout << "\nAges map:" << endl;
    for (const auto& pair : ages) {
        cout << pair.first << " is " << pair.second << " years old" << endl;
    }
    
    // Finding in map
    string name = "Bob";
    if (ages.find(name) != ages.end()) {
        cout << name << " found with age " << ages[name] << endl;
    }
    
    // Using algorithms
    vector<int> nums = {1, 2, 3, 4, 5};
    auto it = find(nums.begin(), nums.end(), 3);
    if (it != nums.end()) {
        cout << "Found 3 at position: " << distance(nums.begin(), it) << endl;
    }
    
    return 0;
}
```

## 12. Exception Handling

```cpp
#include <iostream>
#include <stdexcept>
using namespace std;

class Division {
public:
    static double divide(double a, double b) {
        if (b == 0) {
            throw invalid_argument("Division by zero is not allowed");
        }
        return a / b;
    }
};

class BankAccount {
private:
    double balance;
    
public:
    BankAccount(double initial_balance) : balance(initial_balance) {
        if (initial_balance < 0) {
            throw invalid_argument("Initial balance cannot be negative");
        }
    }
    
    void withdraw(double amount) {
        if (amount > balance) {
            throw runtime_error("Insufficient funds");
        }
        balance -= amount;
    }
    
    double getBalance() const {
        return balance;
    }
};

int main() {
    // Exception handling with division
    try {
        cout << "10 / 2 = " << Division::divide(10, 2) << endl;
        cout << "10 / 0 = " << Division::divide(10, 0) << endl; // This will throw
    } catch (const invalid_argument& e) {
        cout << "Error: " << e.what() << endl;
    }
    
    // Exception handling with bank account
    try {
        BankAccount account(100);
        cout << "Initial balance: $" << account.getBalance() << endl;
        
        account.withdraw(50);
        cout << "After withdrawing $50: $" << account.getBalance() << endl;
        
        account.withdraw(100); // This will throw
    } catch (const runtime_error& e) {
        cout << "Error: " << e.what() << endl;
    } catch (const invalid_argument& e) {
        cout << "Error: " << e.what() << endl;
    } catch (...) {
        cout << "Unknown error occurred" << endl;
    }
    
    return 0;
}
```

## 13. File I/O

```cpp
#include <iostream>
#include <fstream>
#include <string>
using namespace std;

int main() {
    // Writing to file
    ofstream outFile("example.txt");
    if (outFile.is_open()) {
        outFile << "Hello, C++!" << endl;
        outFile << "This is file I/O example." << endl;
        outFile << "Line 3 of the file." << endl;
        outFile.close();
        cout << "Data written to file successfully." << endl;
    } else {
        cout << "Unable to open file for writing." << endl;
        return 1;
    }
    
    // Reading from file
    ifstream inFile("example.txt");
    string line;
    
    if (inFile.is_open()) {
        cout << "\nReading from file:" << endl;
        while (getline(inFile, line)) {
            cout << line << endl;
        }
        inFile.close();
    } else {
        cout << "Unable to open file for reading." << endl;
        return 1;
    }
    
    return 0;
}
```

## 14. Namespace

```cpp
#include <iostream>
using namespace std;

// Custom namespace
namespace MathUtils {
    const double PI = 3.14159;
    
    double circleArea(double radius) {
        return PI * radius * radius;
    }
    
    double circleCircumference(double radius) {
        return 2 * PI * radius;
    }
}

namespace StringUtils {
    string toUpper(string str) {
        for (char& c : str) {
            c = toupper(c);
        }
        return str;
    }
    
    string toLower(string str) {
        for (char& c : str) {
            c = tolower(c);
        }
        return str;
    }
}

int main() {
    double radius = 5.0;
    
    // Using namespace functions
    cout << "Radius: " << radius << endl;
    cout << "Area: " << MathUtils::circleArea(radius) << endl;
    cout << "Circumference: " << MathUtils::circleCircumference(radius) << endl;
    
    string text = "Hello World";
    cout << "\nOriginal: " << text << endl;
    cout << "Uppercase: " << StringUtils::toUpper(text) << endl;
    cout << "Lowercase: " << StringUtils::toLower(text) << endl;
    
    // Using namespace
    using namespace MathUtils;
    cout << "\nUsing namespace - PI value: " << PI << endl;
    
    return 0;
}
```

This comprehensive guide covers the fundamental concepts of both C and C++ programming languages with practical examples. Each section builds upon previous concepts and demonstrates real-world usage patterns.
