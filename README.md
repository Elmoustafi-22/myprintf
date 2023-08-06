# myprintf

`myprintf` is a simple implementation of the `printf` function in C programming language. It allows you to format and print output to the standard output stream (`stdout`) with support for a limited set of conversion specifiers.

## Table of Contents

- [Introduction](#introduction)
	- [Usage](#usage)
	  - [Task 1](#task-1)
	  - [Task 2](#task-2)
	  - [Task 3](#task-3)
	- [Example](#example)
	- [Contributing](#contributing)
	- [License](#license)

## Introduction

	The `myprintf` project aims to provide a simplified version of the `printf` function found in the C standard library. It supports a subset of conversion specifiers, allowing you to print characters, strings, and integer values to the standard output.

## Usage

### Task 1

	In Task 1, you are required to implement a basic version of the `_printf` function that supports the following conversion specifiers:

	- `%c`: Print a single character.
	- `%s`: Print a null-terminated string.
	- `%%`: Print a literal percent character.

	The prototype for the `_printf` function is as follows:

	```c
	int _printf(const char *format, ...);
	```

	The function returns the number of characters printed (excluding the null byte used to end output to strings) and writes output to `stdout`.

### Task 2

	In Task 2, the project expands the `_printf` function to handle additional conversion specifiers:

	- `%d`: Print a signed integer.
	- `%i`: Print an integer.

	Note that for both Task 1 and Task 2, you are not required to handle flag characters, field width, precision, or length modifiers.

### Task 3

	Task 3 introduces custom conversion specifiers:

	- `%b`: Print an unsigned integer in binary form.

	You can use this specifier to print an unsigned integer argument as a binary number.

## Example

	Here's a simple example demonstrating the usage of `myprintf`:

	```c
#include "main.h"
#include <stdio.h>

	int main() {
		    int num = 42;
		        char ch = 'A';
			    char *str = "Hello, world!";
			        
			        int chars_printed = _printf("Integer: %d\nCharacter: %c\nString: %s\nBinary: %b\n", num, ch, str, num);
				    printf("Total characters printed: %d\n", chars_printed);

				        return 0;
	}
```

Output:
```
Integer: 42
Character: A
String: Hello, world!
Binary: 101010
Total characters printed: 55
```

## Contributing

Contributions to `myprintf` are welcome! If you find any bugs, have suggestions for improvements, or want to add new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Note: This documentation provides an overview of the `myprintf` project and its usage. For more detailed information, including code implementation, please refer to the source code in the repository.*
