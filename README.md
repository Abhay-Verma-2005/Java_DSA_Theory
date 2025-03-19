# Arrays in Java

## 1. Declaration of Arrays
### Fixed Size Declaration:
```java
int[] arr = new int[5];
```
### Direct Initialization:
```java
int[] arr2 = {1, 2, 3, 4, 5};
```

## 2. Important Methods in Arrays

### a) Sorting an Array
- **Method:** `Arrays.sort(arr);`
- **Use:** Sorts the array in ascending order.
- **Syntax:**
```java
Arrays.sort(arr);
```

### b) Converting Array to String
- **Method:** `Arrays.toString(arr);`
- **Use:** Converts an array into a readable string format.
- **Syntax:**
```java
String str = Arrays.toString(arr);
```

### c) Filling an Array
- **Method:** `Arrays.fill(arr, value);`
- **Use:** Fills the entire array with the specified value.
- **Syntax:**
```java
Arrays.fill(arr, value);
```

### d) Searching in a Sorted Array (Binary Search)
- **Method:** `Arrays.binarySearch(arr, key);`
- **Use:** Finds the index of the specified element in a sorted array. 
- **Syntax:**
```java
int index = Arrays.binarySearch(arr, key);
```

### e) Copying an Array with New Size
- **Method:** `Arrays.copyOf(arr, newSize);`
- **Use:** Copies the original array into a new array with the specified size.
- **Syntax:**
```java
int[] newArr = Arrays.copyOf(arr, newSize);
```

---
