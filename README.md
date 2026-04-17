# C/C++ Project Template 🚀

A minimalist, high-performance starter template for Windows-based C/C++ development using **MSYS2 (UCRT64)** and **VS Code**.

## 📁 Project Structure

- `.vscode/` - Contains `tasks.json` for automation and build settings.
- `src/` - All your source files (.c, .cpp).
- `build/` - Where your compiled `.exe` files go (this folder is ignored by Git).

## 🛠️ Getting Started

1. **Clone/Use Template:** Click the green "Use this template" button on GitHub to create your own repo.
2. **Open in VS Code:** Open your new project folder in VS Code.
3. **Build Code:** Press `Ctrl + Shift + B`. This will:
   - Automatically create the `build/` folder if it doesn't exist.
   - Compile your active file.
4. **Run Code:** Go to the top menu `Terminal > Run Task...` and select `3. Build and Run`.

## ⚙️ Requirements

- **Compiler:** [MSYS2](https://www.msys2.org/) with the `UCRT64` toolchain.
- **IDE:** [Visual Studio Code](https://code.visualstudio.com/) with the "C/C++" extension by Microsoft.

## ⚠️ Handling "Unused Parameter" Warnings

This template uses professional-grade strict flags (`-Wall -Wextra`) to help you write better code. If you see a warning about `unused parameter 'argc'` or `'argv'`, it means the compiler is doing its job!

**How to fix it:**

- **Option 1: The "Simple C" Way** (Recommended if you don't need arguments):
  ```c
  int main(void) {
      // Your code here
      return 0;
  }
  ```
- **Option 2: The "Professional" Way (If you want to keep the parameters for later):**

  ```c
  int main(int argc, char \*argv[]) {
  (void)argc; // Tell compiler we intentionally aren't using this yet
  (void)argv;

   // Your code here
   return 0;
  ```
