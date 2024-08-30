
# Rush00-Rectangle-Generator

Rush00 is a part of the Hive Helsinki Piscine weekend projects designed to test your understanding of C programming. This exercise aims to create a function that generates various rectangle shapes based on the dimensions provided as input. 

## Structure

- **main.c**: The main file to test the `rush` function.
- **ft_putchar.c**: A utility function used to print a single character to the standard output.
- **rush04.c**: Contains the `rush` function that generates the rectangle shapes.

## Compilation and Usage

```bash
gcc -Wall -Wextra -Werror main.c ft_putchar.c rush04.c -o rush04
```

```bash
./rush04 (num of coluns) (num of lines) # exp ./rush04 5 3
```

## Examples

Here are some examples of what the output should look like with different inputs:

1. **rush(5, 3)**
   ```
   ABBBC
   B   B
   CBBBA
   ```

2. **rush(1, 5)**
   ```
   A
   B
   B
   B
   C
   ```

3. **rush(4, 4)**
   ```
   ABBC
   B  B
   B  B
   CBBA
   ```

## Function Descriptions

### 1. `ft_putchar`

- **File:** `ft_putchar.c`
- **Prototype:** `void ft_putchar(char l);
- This is a utility function that writes a single character to the standard output. It uses the `write` system call to print the character passed as an argument to the console.
- **Parameters:**  
  - `char l`: The character to be printed.

### 2. `main`

- **File:** `main.c`
- **Prototype:** `int main(void);
- Serves as the entry point for the program. It initializes the program by calling the `rush` function with specific dimensions to demonstrate its functionality. This function returns 0 upon successful execution.
- **Parameters:**  
  - None.

### 3. `rush`

- **File:** `rush04.c`
- **Prototype:** `void rush(int x, int y);
- Generates a rectangle shape based on the provided width (`x`) and height (`y`). It first checks if the given dimensions are valid (i.e., both greater than zero) and then calls the `display_lines` function to print the rectangle.
- **Parameters:**  
  - `int x`: The width of the rectangle.
  - `int y`: The height of the rectangle.

### 4. `display_first_line`

- **File:** `rush04.c`
- **Prototype:** `void display_first_line(int x);
- Prints the top border of the rectangle using specific characters. It handles different cases based on the width (`x`) provided, ensuring the correct characters are printed for the rectangle's top line.
- **Parameters:**  
  - `int x`: The width of the rectangle.

### 5. `display_last_line`

- **File:** `rush04.c`
- **Prototype:** `void display_last_line(int x);
- Prints the bottom border of the rectangle using specific characters. Similar to `display_first_line`, it adjusts the output based on the rectangle's width (`x`).
- **Parameters:**  
  - `int x`: The width of the rectangle.

### 6. `display_line_between`

- **File:** `rush04.c`
- **Prototype:** `void display_line_between(int x);
- Prints the middle lines of the rectangle, which consist of border characters at the start and end with spaces in between. It manages different cases based on the width (`x`), ensuring the interior lines are correctly formatted.
- **Parameters:**  
  - `int x`: The width of the rectangle.

### 7. `display_lines`

- **File:** `rush04.c`
- **Prototype:** `void display_lines(int x, int y);
- Coordinates the printing of the entire rectangle by calling `display_first_line`, `display_line_between`, and `display_last_line` as needed based on the given dimensions (`x` and `y`). It manages the overall flow to ensure the rectangle is printed correctly.
- **Parameters:**  
  - `int x`: The width of the rectangle.
  - `int y`: The height of the rectangle.

## Contributors
*[Ilia Munaev](https://www.linkedin.com/in/iliamunaev/)*  
*[Laurens Haas](https://www.linkedin.com/in/laurens-haas-598b64218/)*  
*[Udochukwu Kalusian](https://www.linkedin.com/in/udochukwu-kalusian-246b70282/)*

## License

This project is open-source and available under the MIT License.
