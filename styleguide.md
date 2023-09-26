---
layout: page
title: Style Guide
description: Pointers on how to solve common technical issues.
nav_order: 7
---

# Style Guide 👀
{:.no_toc .fs-7 .fw-400 }

## Style Requirements

You will be graded for the style of programming on this assignment. A few key requirements for style are given below. Here is a complete [Java style guide](https://sp18.datastructur.es/materials/guides/style-guide.html): Java Style Guide written by Alan Yao from UC Berkeley. We will test you on a smaller set of rules:


### **Line Limit**

No line may be longer than 100 characters (the number of characters <= 100).

### **Names**
* Names of static final constants must be in all capitals (e.g., RED, DEFAULT_NAME).
* Names of parameters, local variables, and methods must start with a lower-case letter, or consist of a single, upper-case letter. (e.g., maxLength, N, index, getWidth).
* Names of types (classes), including type parameters, must start with a capital letter (e.g., SampleClass, LinkedList).
* Give all your variable name that describe its meaning and purpose to make your code readable. (For loop variables, it is fine to use i, j, k)
* Avoid "magic numbers" (numbers other than -1, 0, 1) in code by giving them meaningful symbolic names (variable names such as "hundred", "two", "three" are not allowed) and defining them as private static final constants at the top of the class.

### **Indentation & Whitespaces**
* The basic indentation step is 4 spaces. (Do not use horizontal tab characters for indentation.)
* Don't mix tabs and spaces.
* Each file must end with a newline sequence.
* Indent code by the basic indentation step for each block level (blocks are generally enclosed in “{“ and “}”).

### **Comments**

* Include a comment of your name and PID at the top of every file.
* Each class should have javadoc comments briefly explaining the purpose of the class, @author, and @since. 
* Each method should have javadoc comments explaining the behavior, parameters (using @param tag), return type (using @return tag), exception the method throws (using @throws tag).
* You should write inline comments for complicated parts of your code to explain the logic of your code.

### **Example**  SampleClass.java file:

 ```java

    /* 
    * NAME: First Last
    * PID: Axxxxxxxx
    */
    import java.lang.IndexOutOfBoundsException;
    /**
    * Description of Sample Class
    * 
    * @author First Last
    * @since ${date}
    */
    class SampleClass {

    /* Declare constants and magic numbers */
    private static final int MAX_SIZE = 100;

    private int instanceVariable;

    /**
     * Description of constructor
     * @param para Description of para
     */
    public SampleClass(int para) {
        // inline comment here to explain complicated logic to make your code readable
        instanceVariable = para;
    }
    
    /**
     * Description of method
     *
     * @param para1 Description of para1
     * @param para2 Description of para2
     * @return Description of return value
     * @throws IndexOutOfBoundsException when this exception is thrown
     */
    public int sampleMethod(int para1, int para2)
            throws IndexOutOfBoundsException {
        }
    }
```



### ***Exceptions***: We will not deduct points if magic numbers appear in your code in the following scenarios
    1. Checking for mod `n`, where `n` can be any number. You don't have to make a variable for the number `n`.<br>
        ```py 
        number_to_check % 2 == 0  # Example for mod 2
        number_to_check % 3 == 0  # Example for mod 3
         ```
    2. The distance formula (2D & 3D examples are given, but the distance formula is ok for any dimension N).
        ```py
         a ** 2 = b ** 2 + c ** 2              # 2D distance formula
         d ** 2 = x1 ** 2 + x2 ** 2 + x3 ** 2  # 3D distance formula
         ```
    3. Root formulas such as square root, cube root, etc.
        ```py
        square_root = a_number ** (1/2) 
        cube_root   = a_number ** (1/3)
             ```



