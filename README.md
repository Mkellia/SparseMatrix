markdown
Copy code
# SparseMatrix

This project implements basic operations (addition, subtraction, and multiplication) on sparse matrices. The matrices are stored in an optimized data structure to save memory and improve runtime efficiency. This project is designed as a programming assignment for a data structures and algorithms course.

## Directory Structure

The project directory should be organized as follows:

/dsa/sparse_matrix/code/src/ # Source code directory
/dsa/sparse_matrix/input/ # Directory for input files

mathematica
Copy code

## Input File Format

The input files for the sparse matrices should be formatted as follows:

rows=<number_of_rows>
cols=<number_of_columns>
(row_index, col_index, value)
...

mathematica
Copy code

For example:

rows=8433
cols=3180
(0, 381, -694)
(0, 128, -838)
(0, 639, 857)
(0, 165, -933)
(0, 1350, -89)

markdown
Copy code

- The first line specifies the number of rows.
- The second line specifies the number of columns.
- Subsequent lines specify non-zero values in the matrix, with each line containing a tuple `(row_index, col_index, value)`.

## Features

- **Read a sparse matrix from a file**: Parses the input file to create a sparse matrix.
- **Perform matrix operations**:
  - Addition
  - Subtraction
  - Multiplication
- **Custom exception handling**: Handles input file format errors and invalid matrix operations.
- **Memory and runtime optimized data structure**.
- **Write results to file**: Writes the result of the matrix operation to a file named `results.txt`.

## Usage

### Running the Code

1. Ensure you have Python installed on your system.
2. Navigate to the source code directory:

```sh
cd /dsa/sparse_matrix/code/src/
Run the script with the desired input file paths:
sh
Copy code
python main.py <matrix1_path> <matrix2_path>
Example
sh
Copy code
python main.py /dsa/sparse_matrix/input/matrix1.txt /dsa/sparse_matrix/input/matrix2.txt
After running the script, you will be prompted to choose the matrix operation:

markdown
Copy code
Choose the matrix operation:
1. Addition
2. Subtraction
3. Multiplication
Enter the number corresponding to the desired operation (1, 2, or 3). The result will be written to results.txt.

Exception Handling
The code will throw a ValueError with the message "Input file has wrong format" if the input file does not conform to the expected format. It will also raise errors for invalid matrix operations (e.g., attempting to add matrices with different dimensions).

Sample Input Files
Sample input files are provided in the /dsa/sparse_matrix/input/ directory. These files can be used to test the functionality of the code.

Code Documentation
The source code includes comments and documentation to explain the logic and structure of the implementation. Please refer to the comments within the code for detailed explanations.

License
This project is intended for educational purposes and is licensed under the MIT License. Feel free to modify and use the code as needed.

Author
[Your Name]

Feel free to reach out for any questions or clarifications regarding the implementation.

markdown
Copy code

### Tips for Customization

- **Replace placeholders**: Ensure to replace `[Your Name]` with your actual name.
- **Add more details**: Depending on your implementation, you might want to add more sections or details, such as prerequisites, installation steps, or detailed usage examples.
- **Documentation**: If your code has complex logic, consider adding more detailed documentation within your code files.

This setup writes the result of the selected matrix operation to a file called `results.txt` and prints a message to inform the user. The `to_file` method is used to handle writing the result to the file.






