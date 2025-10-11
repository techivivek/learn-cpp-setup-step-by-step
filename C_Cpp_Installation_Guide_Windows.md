# 🚀 Installing C/C++ on Windows (Step-by-Step Guide)

This guide will help you set up a C/C++ development environment on **Windows** using **MinGW** and **Visual Studio Code**.

---

## 🧩 Step 1: Install MinGW

1. Download **MinGW** from the official SourceForge page:  
   👉 [https://sourceforge.net/projects/mingw/](https://sourceforge.net/projects/mingw/)

2. Run the installer and select the following packages:
   - `mingw32-gcc-g++` (C/C++ compiler)
   - `mingw32-base`
   - `mingw32-gcc`

3. Once selected, click **Installation → Apply Changes** to install all packages.

---

## ⚙️ Step 2: Set Up Environment Variables (PATH)

1. Open **File Explorer** → Right-click **This PC** → Select **Properties**.  
2. Click **Advanced system settings** → **Environment Variables**.  
3. Under **System variables**, find and select **Path**, then click **Edit**.  
4. Click **New** and add the following path (adjust if installed elsewhere):

   ```
   C:\MinGW\bin
   ```

5. Click **OK** on all windows to save.

---

## ✅ Step 3: Verify MinGW Installation

Open **Command Prompt (CMD)** and type:

```bash
g++ --version
```

If everything is set up correctly, you’ll see the installed **g++ version** displayed.

---

## 🧰 Step 4: Install Visual Studio Code (VS Code)

If you don’t have VS Code installed yet, download it here:  
👉 [https://go.microsoft.com/fwlink/?LinkID=534107](https://go.microsoft.com/fwlink/?LinkID=534107)

---

## 🔌 Step 5: Install Required VS Code Extensions

Open **VS Code**, then install the following extensions:

1. **C/C++** – by Microsoft (for IntelliSense and debugging)
2. **Code Runner** – by Jun Han (for running code easily)

---

## ▶️ Step 6: Run Your First C/C++ Program

1. Create a new file and save it as `hello.cpp`.
2. Add the following code:

   ```cpp
   #include <iostream>
   using namespace std;

   int main() {
       cout << "Hello, World!" << endl;
       return 0;
   }
   ```

3. Run the program using:
   - **Code Runner** (click ▶️ at the top-right), or  
   - Run manually in terminal:
     ```bash
     g++ hello.cpp -o hello
     ./hello
     ```

---

## 🎉 You’re All Set!

You’ve successfully installed and configured **C/C++** on Windows using **MinGW** and **VS Code**.  
Now you can start building your C/C++ projects with ease.
