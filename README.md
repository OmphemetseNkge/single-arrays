# single-arrays
📦 Module 1 – One Dimensional Arrays | Java tutoring notes by Omphemetse Nkge
### 👤 Tutor: Omphemetse Nkge | Programming Fundamentals

---

## 📌 Overview

An **array** is a collection of a fixed number of variables (called elements or components) that all share the same name and the same data type. Elements are stored in **consecutive memory locations**, and the length of an array is fixed once it is created.

```
int c[] = new int[5];

Index:   c[0]   c[1]   c[2]   c[3]   c[4]
Values:  [ 12 ] [ 34 ] [ 56 ] [ 67 ] [  9 ]
```

---

## 🧠 Table of Contents

- [Introduction](#-introduction)
- [Array Types](#-array-types)
- [Declaring an Array](#-declaring-an-array)
- [Instantiating an Array](#-instantiating-an-array)
- [Initializing & Accessing Elements](#-initializing--accessing-elements)
- [Array Manipulation with Loops](#-array-manipulation-with-loops)
- [Finding Sum & Average](#-finding-sum--average)
- [Finding Largest & Smallest](#-finding-largest--smallest)
- [Array Index Out of Bounds](#-array-index-out-of-bounds)
- [Exercises](#-exercises)

---

## 📖 Introduction

- Elements in an array are accessed using an **index** (also called a subscript), starting at **0**
- The `i`th element is accessed at index `i - 1`
- A subscript can be an integer or an integer expression, e.g., `c[4-2]` evaluates to `c[2]`

```java
int c[] = new int[5];
c[0] = 12;
c[1] = 34;
// The ith element is at c[i-1]
```

---

## 🗂️ Array Types

| Type | Description |
|------|-------------|
| **One-Dimensional** | One row with multiple columns — `c[0], c[1], ..., c[n]` |
| **Two-Dimensional** | Rows and columns (a table/matrix) — `matrix[row][col]` |

---

## 📝 Declaring an Array

```java
// Syntax Option 1
datatype[] arrayName;

// Syntax Option 2
datatype arrayName[];

// Examples
int[] num;
int num[];

// Using a constant for array size
final int ARRAY_SIZE = 12;
int[] arrayName;
arrayName = new int[ARRAY_SIZE];
```

---

## 🏗️ Instantiating an Array

```java
// General syntax
arrayName = new datatype[size];

// Example: array of 10 integers
int[] num;
num = new int[10];
// Elements: num[0], num[1], num[2] ... num[9]
```

---

## ✏️ Initializing & Accessing Elements

```java
// Storing a value
num[3] = 65;   // Value 65 stored at index 3 (4th position)
num[5] = 56;   // Stores 56 at 6th element

// Arithmetic with array elements
num[5] = num[2] + num[3];  // Add elements at index 2 and 3, store in index 5

// Displaying elements
System.out.println(num[3] + "  " + num[4] + "  " + num[0]);

// Initialization during declaration
double[] sales = {12.4, 45.67, 32.90, 78.9, 21.90};

// Partial initialization — remaining elements default to 0
int[] list = new int[10];
// list = {3, 6, 7} → list[0]=3, list[1]=6, list[2]=7, rest are 0
```

---

## 🔁 Array Manipulation with Loops

```java
int[] sales = new int[10];
int index;

// Initializing all elements to 0
for (index = 0; index < 10; index++)
    sales[index] = 0;

// Reading input data into array
for (index = 0; index < 10; index++)
    sales[index] = console.nextInt();

// Printing all elements
for (index = 0; index < 10; index++)
    System.out.println(sales[index] + "   ");
```

> 💡 **Tip:** Use loops when dealing with many values — it avoids writing repetitive code!

---

## ➕ Finding Sum & Average

```java
int[] sales = {5, 6, 7, 8, 9, 10, 11, 12, 13, 14};
int sum = 0;
int average = 0;

for (int index = 0; index < sales.length; index++) {
    sum = sum + sales[index];
}

average = sum / sales.length;
System.out.println("The sum is: " + sum);
System.out.println("The average is: " + average);
```

---

## 🏆 Finding Largest & Smallest

```java
int[] arr = {23, 68, 54, 65, 76, 65, 34};

// Largest element
int largestIndex = 0;
int largeValue = 0;

for (int y = 0; y < arr.length; y++) {
    if (arr[y] >= arr[largestIndex]) {
        largestIndex = y;
        largeValue = arr[largestIndex];
    }
}
System.out.println("Largest number: " + largeValue);

// Smallest element
int minIndex = 0;
int smallestSale;

for (int index = 0; index < arr.length; index++) {
    if (arr[minIndex] > arr[index])
        minIndex = index;
}
smallestSale = arr[minIndex];
```

---

## ⚠️ Array Index Out of Bounds

| Status | Condition |
|--------|-----------|
| ✅ **In Bounds** | `index >= 0` AND `index <= Array_Size - 1` |
| ❌ **Out of Bounds** | `index < 0` OR `index > Array_Size - 1` |

```java
int[] arr = new int[5]; // Valid indices: 0 to 4
arr[5] = 10; // ❌ ArrayIndexOutOfBoundsException!
```

---

## 🧩 Exercises

### Exercise 1 – Product Price Table
A salesman sells 5 products with the following prices:

| Product | Price |
|---------|-------|
| 1 | R14 |
| 2 | R5 |
| 3 | R37 |
| 4 | R8 |
| 5 | R57 |

Write a Java program that:
- ✅ Calculates the **average** price
- ✅ Calculates the **total** price
- ✅ Finds the **largest** price
- ✅ Finds the **lowest** price

---

## 📬 Contact & Tutoring

| | |
|--|--|
| **Tutor** | Omphemetse Nkge |
| **Module** | Programming Fundamentals |
| **Topic** | One Dimensional Arrays |

> *"Arrays are the foundation of data structures — master them and everything else becomes easier."*
> — Omphemetse Nkge

