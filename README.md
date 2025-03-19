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

#### Example:
```java
import java.util.Arrays;

public class Main {
    public static void main(String[] args) {
        int[] arr = {5, 3, 1, 4, 2};
        Arrays.sort(arr);
        System.out.println(Arrays.toString(arr));  // Output: [1, 2, 3, 4, 5]
    }
}
```

### b) Converting Array to String
- **Method:** `Arrays.toString(arr);`
- **Use:** Converts an array into a readable string format.

#### Example:
```java
import java.util.Arrays;

public class Main {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 4, 5};
        String str = Arrays.toString(arr);
        System.out.println(str);  // Output: [1, 2, 3, 4, 5]
    }
}
```

### c) Filling an Array
- **Method:** `Arrays.fill(arr, value);`
- **Use:** Fills the entire array with the specified value.

#### Example:
```java
import java.util.Arrays;

public class Main {
    public static void main(String[] args) {
        int[] arr = new int[5];
        Arrays.fill(arr, 10);
        System.out.println(Arrays.toString(arr));  // Output: [10, 10, 10, 10, 10]
    }
}
```

### d) Searching in a Sorted Array (Binary Search)
- **Method:** `Arrays.binarySearch(arr, key);`
- **Use:** Finds the index of the specified element in a sorted array.
- (requires the array to be **sorted** before searching.)

#### Example:
```java
import java.util.Arrays;

public class Main {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 4, 5};
        int index = Arrays.binarySearch(arr, 3);
        System.out.println(index);  // Output: 2
    }
}
```

### e) Copying an Array with New Size
- **Method:** `Arrays.copyOf(arr, newSize);`
- **Use:** Copies the original array into a new array with the specified size.

#### Example:
```java
import java.util.Arrays;

public class Main {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 4, 5};
        int[] newArr = Arrays.copyOf(arr, 10);
        System.out.println(Arrays.toString(newArr));  
        // Output: [1, 2, 3, 4, 5, 0, 0, 0, 0, 0]
    }
}
``` 
