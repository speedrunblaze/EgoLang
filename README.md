# Ego Programming Language Documentation

The Ego language is a high-level programming language. It is simple and focuses on basic tasks like declaring variables, printing values, and using conditionals for flow control.

#

### **Language Structure**

#### 1. **Variable Declarations**

Variables can be declared using two keywords: `public` and `private`.  
- `public` variables can be accessed anywhere in the program.  
- `private` variables can only be accessed in the block where they are declared.  

You can also use `mutable` or `immutable`:  
- `mutable`: The variable can be changed after it is declared.  
- `immutable`: The variable cannot be changed after it is declared.  

**Syntax:**  
```ego
public mutable <type> <variable_name> = <value>;
private immutable <type> <variable_name> = <value>;
```

**Example:**  
```ego
public mutable int a = 10;
private immutable int b = 5;
```

#

#### 2. **Data Types**

Ego supports these data types:  
- `int`: For whole numbers (e.g., 10, -5).  
- `float`: For decimal numbers (e.g., 3.14, -0.5).  
- `string`: For text (e.g., "Hello").  

**Example:**  
```ego
public mutable int age = 30;
private immutable string name = "John";
```

# 

#### 3. **Assignments**

You can assign values to variables using the `=` sign.  

**Syntax:**  
```ego
<variable_name> = <value>;
```

**Example:**  
```ego
a = 20;
```

#

#### 4. **Print Command**

To print values or messages, use the `print()` command.  

**Syntax:**  
```ego
print(<variable_or_text>);
```

**Example:**  
```ego
print(a);
print("Hello, World!");
```

#

#### 5. **Conditionals (if-else)**

Ego supports `if-else` for decision-making.  

**Syntax:**  
```ego
if (<condition>) {
    <if_block>;
} else {
    <else_block>;
}
```

- `condition`: A true/false expression.  
- `if_block`: Code to run if the condition is true.  
- `else_block`: Code to run if the condition is false.  

**Example:**  
```ego
if (a > 10) {
    print("The variable a is greater than 10");
} else {
    print("The variable a is not greater than 10");
}
```

#

#### 6. **Operators**

Ego supports these operators:  

**Arithmetic:**  
- `+`: Addition  
- `-`: Subtraction  
- `*`: Multiplication  
- `/`: Division  
- `%`: Modulus (remainder of division)  

**Example:**  
```ego
public mutable int sum = a + b;
public mutable float division = a / 2.0;
```

**Comparison:**  
- `==`: Equal to  
- `!=`: Not equal to  
- `>`: Greater than  
- `<`: Less than  
- `>=`: Greater than or equal to  
- `<=`: Less than or equal to  

**Example:**  
```ego
if (a == b) {
    print("The variables are equal");
} else {
    print("The variables are different");
}
```

**Logical:**  
- `&&`: AND  
- `||`: OR  
- `!`: NOT  

**Example:**  
```ego
if (a > 10 && b < 20) {
    print("Both conditions are true");
}
```
#

#### 7. **Comments**

Comments are used to explain code and are ignored during execution.  

- Single-line comment: Starts with `//`.  
- Multi-line comment: Starts with `/*` and ends with `*/`.  

**Example:**  
```ego
// This is a single-line comment
/*
This is a multi-line comment
spanning multiple lines
*/
```

---

### **Full Example**

Here is a simple Ego program:  

```ego
public mutable int a = 10;
private immutable int b = 5;
public mutable int result = a + b;

print(result);

if (result > 10) {
    print("The result is greater than 10");
} else {
    print("The result is 10 or less");
}
```

**Explanation:**  
1. Declare variables `a`, `b`, and `result`.  
2. Print the value of `result`.  
3. Check if `result` is greater than 10 and print a message.  

#

### **Final Thoughts**

Ego is a simple and powerful language, perfect for beginners or projects that need basic features like variables, conditionals, and math operations. It is easy to learn and use.
