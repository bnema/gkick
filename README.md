# Go Echo HTMX Kickstart project

## Overview

This is my kickstart project for building web applications. The stack is minimalist and includes the following:

- **Embedding**: Embed static folder and templates into the binary.
- **HTMX**: Enables dynamic content updates without requiring a full page reload.
- **Hyperscript**: Simplifies frontend interactivity with syntactic sugar.
- **Go Templates Rendering**: HTML rendering with Go's standard library.
- **Tailwind CSS**: Integrated for utility-first CSS styling (because i'm too lazy to write CSS).
- **Air for Hot Reloading**: Enables a smooth development experience by automatically reloading the application on code changes.
  
The project also aims to maintain a structure that aligns with Golang's standard project layout.

## Getting Started

1. **Clone the repository.**

    ```
    git clone https://github.com/bnema/kickstart-echo.git .
    ```
2. **Install dependencies.**
    ```
    go mod tidy
    ```
3. **Remove the Git History.**
    ```
    rm -rf .git
    ```
4. **Create a .env at the root of the project and add a SESSION_SECRET.**
   ```
    SESSION_SECRET=your-secret-here
    ```
5. **Install Air for Hot Reloading.**
    Follow the [Air installation guide](https://github.com/cosmtrek/air).
6. **Install Bun for Tailwind CSS.**
    Follow the [Bun installation guide](https://bun.sh/docs/installation).
7. **Run Bun Install.**
    ```
    bun install
    ```
8. **Execute Tailwind with Bun.**
    ```
    bun run dev:css
    ```
9. **Run the Application (Air will rebuild and restart the application on code changes).**
    ```
    air
    ```

## License
Under the GPL-3.0 license. Please see the LICENSE file for more details.