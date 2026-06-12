# 00 - Getting Started with Java

Welcome to Level 1 of the Java Learning Program! Before we dive into learning Java, let's make sure your development environment is properly set up.

## 🎯 What You'll Do Today

1. Install Java Development Kit (JDK)
2. Install a code editor
3. Write and run your first Java program
4. Verify everything is working

---

## 📦 Step 1: Install Java Development Kit (JDK)

Java requires the **JDK (Java Development Kit)** to compile and run programs. We recommend **JDK 17 LTS** (Long Term Support).

### Option A: Oracle JDK (Official)
1. Visit: https://www.oracle.com/java/technologies/downloads/
2. Click "JDK 17" → Download for your operating system
3. Follow the installation wizard
4. Accept the default installation location

### Option B: OpenJDK (Free Alternative)
1. Visit: https://openjdk.org/install/
2. Follow instructions for your OS
3. Complete the installation

### Verify Installation

After installation, open your terminal/command prompt and type:
```bash
java -version
```

**Expected Output** (something like this):
```
java version "17.0.6" 2023-01-17 LTS
Java(TM) SE Runtime Environment (build 17.0.6+10-LTS-190)
Java HotSpot(TM) 64-Bit Server VM (build 17.0.6+10-LTS-190, mixed mode, sharing)
```

If you see this, ✅ **Java is correctly installed!**

If you get an error like `java: command not found`, reinstall Java and make sure it's added to your system PATH.

---

## 💻 Step 2: Install a Code Editor

You need a text editor to write Java code. Choose one:

### ✅ Recommended: IntelliJ IDEA Community (FREE)
- **Download:** https://www.jetbrains.com/idea/download/
- **Pros:** Best for Java, lots of features, easy to use
- **Steps:** Download → Install → Open → Create New Project

### ✅ Alternative: VS Code (FREE)
- **Download:** https://code.visualstudio.com/
- **Pros:** Lightweight, free, works with any language
- **Setup:** 
  1. Install Extension Packs for Java (by Microsoft)
  2. You're ready to code

### ✅ Alternative: Eclipse (FREE)
- **Download:** https://www.eclipse.org/downloads/
- **Pros:** Popular, full-featured IDE for Java
- **Steps:** Download → Install → Open

**For this course, we recommend VS Code or IntelliJ IDEA.**

---

## 🚀 Step 3: Write Your First Java Program

### Create a folder for your code:
```bash
mkdir java-learning
cd java-learning
```

### Create a file called `HelloWorld.java`:

**In VS Code:**
1. Open VS Code
2. File → Open Folder → Select `java-learning`
3. Click New File → Name it `HelloWorld.java`
4. Type the code below:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### Save the file

---

## ▶️ Step 4: Compile and Run Your Program

### In Terminal/Command Prompt:

**Compile the program:**
```bash
javac HelloWorld.java
```

This creates a `HelloWorld.class` file (the compiled version).

**Run the program:**
```bash
java HelloWorld
```

**Expected Output:**
```
Hello, World!
```

🎉 **Congratulations! Your first Java program works!**

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| `javac: command not found` | Java is not installed or not in PATH. Reinstall Java. |
| `Error: Could not find or load main class HelloWorld` | Make sure the file is named exactly `HelloWorld.java` and is in the current directory. |
| `ClassName does not match filename` | The public class name must match the filename exactly. |
| Program doesn't print anything | Check for typos in `System.out.println()` |

---

## 📝 Understanding the Code

Let's break down the `HelloWorld.java` program:

```java
public class HelloWorld {           // Declare a public class named HelloWorld
    public static void main(String[] args) {  // The entry point of the program
        System.out.println("Hello, World!");   // Print text to console
    }
}
```

**Key Points:**
- `public class HelloWorld` - Defines a class. File must be named `HelloWorld.java`
- `public static void main(String[] args)` - Special method where Java starts running your program
- `System.out.println()` - Prints text followed by a new line

---

## ✅ You're Ready!

If you can run `HelloWorld.java` and see the output, you're all set to start learning Java!

**Next Step:** Read [01-Introduction.md](01-Introduction.md)

---

## 🎓 Key Takeaways

- ✅ Java needs to be installed via JDK
- ✅ You need a code editor to write Java
- ✅ Java code must be compiled before running
- ✅ Your first program works!

**Ready to continue? Let's go to Lesson 1!** →

