# Java Data Structures Guide
[Check Here](https://javaes.netlify.app/)
---

## Table of Contents
1. [Arrays in Java](#arrays-in-java)
2. [Strings in Java](#strings-in-java)
3. [StringBuilder in Java](#stringbuilder-in-java)
4. [ArrayList in Java](#arraylist-in-java)
5. [HashSet in Java](#hashset-in-java)
6. [HashMap in Java](#hashmap-in-java)
7. [LinkedList in Java](#linkedlist-in-java)

---

## Arrays in Java

### Declaration of Arrays
#### Fixed Size Declaration:
```java
int[] arr = new int[5];
```
#### Direct Initialization:
```java
int[] arr2 = {1, 2, 3, 4, 5};
```

### Important Methods in Arrays

#### a) Sorting an Array
- **Method:** `Arrays.sort(arr);`
- **Use:** Sorts the array in ascending order.
- **Syntax:**
```java
Arrays.sort(arr);
```

#### b) Converting Array to String
- **Method:** `Arrays.toString(arr);`
- **Use:** Converts an array into a readable string format.
- **Syntax:**
```java
String str = Arrays.toString(arr);
```

#### c) Filling an Array
- **Method:** `Arrays.fill(arr, value);`
- **Use:** Fills the entire array with the specified value.
- **Syntax:**
```java
Arrays.fill(arr, value);
```

#### d) Searching in a Sorted Array (Binary Search)
- **Method:** `Arrays.binarySearch(arr, key);`
- **Use:** Finds the index of the specified element in a sorted array. 
- **Syntax:**
```java
int index = Arrays.binarySearch(arr, key);
```

#### e) Copying an Array with New Size
- **Method:** `Arrays.copyOf(arr, newSize);`
- **Use:** Copies the original array into a new array with the specified size.
- **Syntax:**
```java
int[] newArr = Arrays.copyOf(arr, newSize);
```

---

## Strings in Java

### Declaration of Strings
- **Literal Declaration:** `String s = "Hello";`
- **Object Creation:** `String s2 = new String("World");`

### Important Methods in Strings

#### a) Get Length of a String
- **Method:** Returns the number of characters in the string.
```java
s.length();
```

#### b) Get Character at a Specific Index
- **Method:** Fetches the character at the given index.
```java
s.charAt(index);
```

#### c) Convert to Uppercase
- **Method:** Converts all characters to uppercase.
```java
s.toUpperCase();
```

#### d) Convert to Lowercase
- **Method:** Converts all characters to lowercase.
```java
s.toLowerCase();
```

#### e) Check if String Contains a Substring
- **Method:** Returns `true` if the string contains the given substring.
```java
s.contains("substring");
```

#### f) Compare Two Strings
- **Method:** Checks if two strings are equal.
```java
s.equals(s2);
```

#### g) Concatenate Two Strings
- **Method:** Joins the current string with another string.
```java
s.concat(" anotherString");
```

#### h) Replace Characters in a String
- **Method:** Replaces all occurrences of a character with another.
```java
s.replace('oldChar', 'newChar');
```

#### i) Remove Leading & Trailing Spaces
- **Method:** Trims whitespace from both ends of the string.
```java
s.trim();
```

#### j) Split a String
- **Method:** Splits the string based on a specified delimiter.
```java
s.split("delimiter");
```

#### k) Extract a Substring
- **Method:** Returns a part of the string from the given index range.
```java
s.substring(startIndex);
s.substring(startIndex, endIndex);
```

---

## StringBuilder in Java

### Declaration of StringBuilder
- **Using Constructor:**
```java
StringBuilder sb = new StringBuilder("Hello");
```

### Important Methods in StringBuilder

#### a) Append a String
- **Method:** Adds the given string at the end.
```java
sb.append(" World");
```

#### b) Insert at a Specific Position
- **Method:** Inserts a string at the specified index.
```java
sb.insert(index, "text");
```

#### c) Replace a Substring
- **Method:** Replaces a portion of the string between given indexes.
```java
sb.replace(startIndex, endIndex, "newText");
```

#### d) Delete Part of a String
- **Method:** Removes characters from the specified range.
```java
sb.delete(startIndex, endIndex);
```

#### e) Reverse the String
- **Method:** Reverses the entire string.
```java
sb.reverse();
```

#### f) Get Length of StringBuilder
- **Method:** Returns the number of characters in the StringBuilder.
```java
sb.length();
```

#### g) Convert StringBuilder to String
- **Method:** Converts StringBuilder to a regular string.
```java
sb.toString();
```

---

## ArrayList in Java

### Declaration of ArrayList
- **Integer List:**
```java
ArrayList<Integer> list = new ArrayList<>();
```
- **String List:**
```java
ArrayList<String> strList = new ArrayList<>();
```
- **Boolean List:**
```java
ArrayList<Boolean> boolList = new ArrayList<>();
```

### Important Methods in ArrayList

#### a) Add an Element
- **Method:** Adds an element to the list.
```java
list.add(value);
```

#### b) Get an Element
- **Method:** Retrieves the element at the specified index.
```java
list.get(index);
```

#### c) Update an Element
- **Method:** Updates the value at the given index.
```java
list.set(index, newValue);
```

#### d) Remove an Element by Index
- **Method:** Removes the element at the given index.
```java
list.remove(index);
```

#### e) Get Size of the ArrayList
- **Method:** Returns the number of elements in the list.
```java
list.size();
```

#### f) Check if an Element Exists
- **Method:** Returns `true` if the element is present.
```java
list.contains(value);
```

#### g) Get Index of an Element
- **Method:** Returns the index of the specified element, or `-1` if not found.
```java
list.indexOf(value);
```

#### h) Clear All Elements
- **Method:** Removes all elements from the list.
```java
list.clear();
```

---

## HashSet in Java

### Declaration of HashSet
- **Integer HashSet:**
```java
HashSet<Integer> set = new HashSet<>();
```

### Important Methods in HashSet

#### a) Add an Element
- **Method:** Adds an element to the set. Duplicates are not allowed.
```java
set.add(value);
```

#### b) Check if an Element Exists
- **Method:** Returns `true` if the element is present in the set.
```java
set.contains(value);
```

#### c) Remove an Element
- **Method:** Removes the specified element from the set.
```java
set.remove(value);
```

#### d) Get Size of the HashSet
- **Method:** Returns the number of elements in the set.
```java
set.size();
```

#### e) Check if the HashSet is Empty
- **Method:** Returns `true` if the set is empty.
```java
set.isEmpty();
```

#### f) Clear All Elements
- **Method:** Removes all elements from the set.
```java
set.clear();
```

---

## HashMap in Java

### Declaration of HashMap
- **Integer Key, String Value:**
```java
HashMap<Integer, String> map1 = new HashMap<>();
```
- **String Key, Integer Value:**
```java
HashMap<String, Integer> map2 = new HashMap<>();
```
- **Boolean Key, Double Value:**
```java
HashMap<Boolean, Double> map3 = new HashMap<>();
```

### Important Methods in HashMap

#### a) Add a Key-Value Pair
- **Method:** Inserts a key-value pair into the HashMap.
```java
map1.put(key, value);
```

#### b) Get a Value by Key
- **Method:** Retrieves the value associated with a given key.
```java
map1.get(key);
```

#### c) Check if a Key Exists
- **Method:** Returns `true` if the key is present in the HashMap.
```java
map1.containsKey(key);
```

#### d) Check if a Value Exists
- **Method:** Returns `true` if the specified value is in the HashMap.
```java
map1.containsValue(value);
```

#### e) Remove a Key-Value Pair
- **Method:** Deletes the key and its associated value.
```java
map1.remove(key);
```

#### f) Get Size of the HashMap
- **Method:** Returns the number of key-value pairs in the HashMap.
```java
map1.size();
```

#### g) Clear All Entries
- **Method:** Removes all key-value pairs from the HashMap.
```java
map1.clear();
```

#### h) Get All Keys
- **Method:** Returns a set of all keys in the HashMap.
```java
map1.keySet();
```

#### i) Get All Values
- **Method:** Returns a collection of all values in the HashMap.
```java
map1.values();
```

---

## LinkedList in Java

### Declaration of LinkedList
- **Integer LinkedList:**
```java
LinkedList<Integer> linkedList = new LinkedList<>();
```

### Important Methods in LinkedList

#### a) Add an Element
- **Method:** Adds an element to the LinkedList.
```java
linkedList.add(value);
```

#### b) Add Element at the Beginning
- **Method:** Inserts an element at the start of the LinkedList.
```java
linkedList.addFirst(value);
```

#### c) Add Element at the End
- **Method:** Inserts an element at the end of the LinkedList.
```java
linkedList.addLast(value);
```

#### d) Get First Element
- **Method:** Retrieves the first element of the LinkedList.
```java
linkedList.getFirst();
```

#### e) Get Last Element
- **Method:** Retrieves the last element of the LinkedList.
```java
linkedList.getLast();
```

#### f) Remove First Element
- **Method:** Deletes the first element from the LinkedList.
```java
linkedList.removeFirst();
```

#### g) Remove Last Element
- **Method:** Deletes the last element from the LinkedList.
```java
linkedList.removeLast();
```

#### h) Check if an Element Exists
- **Method:** Returns `true` if the element is present in the LinkedList.
```java
linkedList.contains(value);
```

#### i) Get Size of the LinkedList
- **Method:** Returns the number of elements in the LinkedList.
```java
linkedList.size();
```

#### j) Creating a Custom display() Method
- If you need a display() method, you can implement it like this:
```java
public void display(LinkedList<Integer> list) {
    for (Integer num : list) {
        System.out.print(num + " ");
    }
    System.out.println();
}
```
**Call it as:**
```java
display(linkedList);
```
