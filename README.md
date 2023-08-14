# MyPrintf - Custom Implementation of printf()

---

MyPrintf is a simple custom implementation of the `printf()` function in C programming language. The `printf()` function is a standard library function used to print formatted output to the console. This project aims to provide a basic version of the `printf()` function, allowing users to print formatted text to the console using a subset of format specifiers.

## Features

- Support for basic format specifiers: `%d`, `%s`, `%c`, `%f`.
- Limited precision and width specification.
- Left-justification and zero-padding options.
- Error handling for unsupported format specifiers.

## Usage

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/Elmoustafi-22/myprintf.git
   ```

2. Navigate to the project directory:

   ```bash
   cd myprintf
   ```
3. Include the `_printf()` and `main.h` files in your C project

4. Use the `_printf()` function to print formatted output:

   ```c
   #include "main.h"

   int main()
   {
	   int num = 42;
	   char str = "Hello, MyPrintf!";

	   _printf("Integer: %d\n", num);
	   _printf("String: %s\n", str);

	   return (0);
   }
   ```
5. Compile your project including the `_printf.c`file:

    ```bash
    gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o print
    ```
6. Run the compile program:

   ```bash
   ./print
   ```

## Format Specifiers

- `%d`: Print an integer.
- `%s`: Print a string.
- `%c`: Prints a character.
- `%f`: Print a floating-point number.

## Limitations

- The implementation supports only a subset of the features of the standard `printf()` function.
- Precision and width specification are limited and might not behave exactly like the stardard `printf()`
- Floating-point numbers are printed using basic formatting and might not have the same precision as the standard `printf()`.

## Contribution

Contributions to this project are welcome! If you find any bugs, have suggestions, or would like to add more features, please feel free to create issues or submit pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/Elmoustafi-22/myprintf/blob/main/LICENSE) file for more details.

---

**Note**: This project is intended for educational and illustrative purposes.
