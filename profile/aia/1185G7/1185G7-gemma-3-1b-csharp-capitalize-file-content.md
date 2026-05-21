```csharp
using System;
using System.IO;

public class FileProcessor
{
    public static void CapitalizeAndSaveFile(string inputFilePath, string outputFilePath)
    {
        try
        {
            // Read the file's contents
            string content = File.ReadAllText(inputFilePath);

            // Capitalize all lowercase letters
            content = content.ToUpper();

            // Write the capitalized content to a new file
            File.WriteAllText(outputFilePath, content); 
            Console.WriteLine($"Successfully capitalized and saved to: {outputFilePath}");
        }
        catch (Exception ex)
        {
            Console.WriteLine($"An error occurred while processing the file: {ex.Message}");
        }
    }

    public static void Main(string[] args)
    {
        // Example usage
        string inputFile = "input.txt"; // Replace with your input file path
        string outputFile = "output.txt"; // Replace with your desired output file path

        CapitalizeAndSaveFile(inputFile, outputFile);
    }
}
```

**Explanation:**

1. **`using System;` and `using System.IO;`**:  These lines import the necessary namespaces for working with files and input/output operations.
2. **`CapitalizeAndSaveFile(string inputFilePath, string outputFilePath)`**: This defines a public static method named `CapitalizeAndSaveFile` that takes two string arguments:
   - `inputFilePath`: The path to the file you want to read.
   - `outputFilePath`: The path where you want to save the capitalized content.

3. **`try...catch`**:  This is a crucial error handling mechanism. It allows the method to gracefully handle potential errors (like file not found, permissions issues, etc.) without crashing the program.

4. **`File.ReadAllText(inputFilePath)`**: This reads the entire contents of the `inputFilePath` string into a string variable named `content`.

5. **`content = content.ToUpper()`**:  This converts the entire `content` string to uppercase using the `ToUpper()` method.

6. **`File.WriteAllText(outputFilePath, content)`**: This writes the capitalized content to the specified `outputFilePath` file. The `WriteAllText` method creates a new text file and writes all of the data from the input stream to it.  Important: It *overwrites* the file if it already exists.

7. **`Console.WriteLine(...)`**: This prints a message to the console indicating that the operation was successful or an error occurred.

8. **`Main(string[] args)`:**  This is the entry point of the program.
   - `string inputFile = "input.txt";`: Sets the path to your input file (you should replace `"input.txt"` with the actual path).
   - `string outputFile = "output.txt";`: Sets the path where you want to save the capitalized content.
   -  `CapitalizeAndSaveFile(inputFile, outputFile);`: Calls the method to perform the file processing and saving.

**How to use this code:**

1. **Create a C# Console Application Project:** In Visual Studio (or your preferred IDE), create a new "Console App" project.
2. **Replace `input.txt` with an actual file:**  Create a text file named `input.txt` in the same directory as your `.cs` file.  Put some lowercase text into this file for testing.
3. **Modify `inputFile` and `outputFile`:** In the code, change the values of `inputFile` to the correct path to your input file and `outputFile` to the desired path for the output file.
4. **Build and Run:** Build the project (usually by pressing Ctrl+Shift+B) and run it in Visual Studio (or your IDE). The capitalized content will be written to the specified output file.

**Important Considerations:**

* **Error Handling**:  The `try...catch` block is essential for robust code. Always include error handling when reading or writing files.
* **File Paths**: Double-check that the paths are correct and that the file exists in the specified location. Use absolute paths if necessary to avoid confusion.
* **Overwriting:** The `WriteAllText` method *overwrites* the output file if it already exists.  If you want to append to an existing file, use the `AppendFile` method instead (but be careful with this – you'll need to handle potential errors).
* **Character Encoding**: If your input file uses a specific character encoding (e.g., UTF-8), make sure to specify that in the `File.ReadAllText()` and `File.WriteAllText()` methods using the appropriate `Encoding` parameter.  If you don't specify an encoding, it will use the system's default encoding, which might not be what you want.