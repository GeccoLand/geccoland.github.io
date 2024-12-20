# Creating Your First Program

Welcome to Gecco! This guide will help you write, compile, and run your first program in Gecco. Let’s dive in!

---

## Step 1: Setting Up Your Environment

Before you begin, make sure:
1. Gecco is installed on your system. (Refer to the [Installation Guide]() for instructions.)
2. Your terminal or IDE is configured to use Gecco's compiler and tools.

---

## Step 2: Writing Your First Program

Let’s start with the classic "Hello, World!" program. Open your preferred text editor or IDE and create a new file named `hello.gec`.

### Example Code: `hello.gec`

```
class Main {
    // Entry point of the program
    static func main() {
        print "Hello, World!"
    }
}
```

### Explanation
- **`class Main {}`**: Defines the `Main` class, which is the starting point of your program.
- **`static func main()`**: The `main` function serves as the program's entry point.
- **`print`**: A built-in function to print text to the console.

---

## Step 3: Compiling Your Program

To compile your program:
1. Open a terminal or command prompt.
2. Navigate to the directory containing `hello.gec`.
3. Run the Gecco compiler:

   ```bash
   gecco-compiler hello.gec -o hello
   ```

   This will generate an executable file named `hello` in the same directory.

---

## Step 4: Running Your Program

Run the compiled program with the following command:

### On Windows:
```bash
hello.exe
```

### On Linux/macOS:
```bash
./hello
```

You should see the output:
```
Hello, World!
```

---

## Step 5: Exploring Further

Now that you've successfully created and run your first program in Gecco, here are some ideas for what to try next:
- Modify the message in `println` to display your name or a custom greeting.
- Experiment with variables and loops (see the [Language Basics](#) page for more examples).
- Build a program that takes user input and prints it back to the console.

Congratulations! You’ve just written your first Gecco program. 🎉

---

Need help? Check out our [Community Forum](#) or [Troubleshooting Guide](#).
