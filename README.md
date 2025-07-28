# 🛠️ OpenGL Starter Pack

This is a ready-to-use OpenGL development setup using **GLAD** (OpenGL Loader) and **GLFW** (Window Management) libraries. The project is pre-configured and ready to build on Windows with MinGW64.

## What's Included

- **GLAD** - Modern OpenGL function loader
- **GLFW** - Cross-platform windowing library
- **Pre-compiled libraries** for 64-bit Windows
- **Sample program**
- **Ready-to-use build configuration**

## Project Structure

<pre>📁 opengl-setup/
├──📁 include/        
│   ├──📁 glad/  
│   ├──📁 GLFW/  
│   └──📁 KHR/   
├──📁 lib/
│   └── libglfw3dll.a
├──📁 src/
│   ├── main.cpp 
│   └── glad.c        
├──📁 .vscode/   
│   └── tasks.json 
├── glfw3.dll
└── README.md     
</pre>

## Quick Start

### Prerequisites

- **MinGW64** (64-bit version)
- **VS Code**

### Step 1: Clone the Repository

```bash
git clone https://github.com/anurag-adk/opengl-setup.git
cd opengl-setup
```

### Step 2: Build the Project

#### Option A: Using VS Code (Recommended)

1. Open the project folder in VS Code
2. Press `Ctrl + Shift + B`

#### Option B: Using Command Line

```bash
# Navigate to project directory
cd opengl-setup

# Build using MinGW64
C:/MingW/mingw64/bin/g++.exe -O2 -std=c++17 -I./include -L./lib ./src/main.cpp ./src/glad.c -lglfw3dll -lopengl32 -lgdi32 -luser32 -lkernel32 -o main.exe
```

### Step 3: Run the Program

```bash
./main.exe
```

You should see a window displaying "HELLO WORLD" in outlined block letters!

## Build Configuration

The project uses a **VS Code task** configured in `.vscode/tasks.json`:

- **Compiler**: MinGW64 g++
- **Standard**: C++17
- **Libraries**: GLFW3, OpenGL32, GDI32, User32, Kernel32
- **Output**: Executable file `.exe` in root of project

## Extending the Project

This setup is ideal for:

- **Learning OpenGL**
- **Graphics programming**
- **Game or rendering projects**
- **Experimenting with shaders**

Feel free to use it as a foundation for your own OpenGL applications.

## 🎉 Happy Coding!

_For queries or feedback, feel free to reach out to me at [iamanuragadhikari@gmail.com](mailto:iamanuragadhikari@gmail.com)_
