# shaankproject
This is my new Git Repository.
<br>
Author-Shaan Khan
<br>
this the new commit...
<br>
I'm working on vs code and git...
<br>
Here’s a simple C++ program that functions as an arithmetic calculator. It supports basic operations: addition, subtraction, multiplication, and division.

```cpp
#include <iostream>

using namespace std;

int main() {
    char operation;
    float num1, num2;

    // Display menu
    cout << "Select an operation (+, -, *, /): ";
    cin >> operation;

    // Get input numbers
    cout << "Enter two numbers: ";
    cin >> num1 >> num2;

    switch(operation) {
        case '+':
            cout << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0) {
                cout << num1 << " / " << num2 << " = " << num1 / num2 << endl;
            } else {
                cout << "Error! Division by zero is not allowed." << endl;
            }
            break;
        default:
            cout << "Error! The operation is not correct." << endl;
            break;
    }

    return 0;
}
```

### How the Program Works:
1. **Operation Selection:** The program asks the user to select an arithmetic operation (`+`, `-`, `*`, or `/`).
2. **Input Numbers:** It then asks for two numbers to perform the operation.
3. **Switch Statement:** Depending on the chosen operation, it performs the corresponding arithmetic operation.
4. **Division by Zero:** It handles the case where the user tries to divide by zero by displaying an error message.
5. **Error Handling:** If the user enters an invalid operation, it shows an error message.

### Example Usage:
- If you input `+` and then `4` and `2`, the output will be:
  ```
  4 + 2 = 6
  ```
- If you input `/` and then `4` and `0`, the output will be:
  ```
  Error! Division by zero is not allowed.
  ```

This program is a good starting point and can be expanded further to include more features or error handling as needed.
