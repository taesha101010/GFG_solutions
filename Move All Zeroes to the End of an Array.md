## 01. Move All Zeroes to the End of an Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/move-all-zeroes-to-end-of-array0751/1)

### Problem Description

**Task:** Given an array arr[] of non-negative integers, move all the zeros to the end of the array while maintaining the relative order of the non-zero elements. Perform the operation in place, without using an extra array.Examples:Input: arr[] = [1, 2, 0, 4, 3, 0, 5, 0]

#### Examples

##### Example 1

- **Output:**
```text
[1, 2, 4, 3, 5, 0, 0, 0]
```
- **Explanation:** The three zeros are moved to the end while the order of the non-zero elements remains unchanged.

##### Example 2

- **Input:**
```text
arr[] = [10, 20, 30]
```
- **Output:**
```text
[10, 20, 30]
```
- **Explanation:** No change in array as there are no 0s.

##### Example 3

- **Input:**
```text
arr[] = [0, 0]
```
- **Output:**
```text
[0, 0]
```
- **Explanation:** No change in array as there are all 0s.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (Java)

- **Submitted:** 2026-11-20 15:42:37
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    void pushZerosToEnd(int[] arr) {
        int j = 0;
        for (int i = 0 ; i < arr.length; i++){
            if(arr[i] != 0){
                if(i != j){
                    arr[j] = arr[i];
                    arr[i] = 0;
                    
                }
                
                j++;
            }
        }
    }
}
```

#### Solution 2 (Java)

- **Submitted:** 2026-11-20 15:26:49
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    void pushZerosToEnd(int[] arr) {
        int j = 0;
        for (int i = 0 ; i < arr.length; i++){
            if(arr[i] != 0){
                if(i != j){
                    arr[j] = arr[i];
                    arr[i] = 0;
                    
                }
                
                j++;
            }
        }
    }
}
```

#### Solution 3 (Java)

- **Submitted:** 2026-11-20 15:01:57
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    void pushZerosToEnd(int[] arr) {
        int j = 0;
        for (int i = 0; i < arr.length; i++){
            if (arr[i] !=0 ){
                if (i != j){
                    arr[j] = arr[i];
                    arr[i] = 0;
                }
                j++;
            }
        }
        
    }
}
```

*Generated on: 20/11/2026, 3:43:04 pm*