## 01. Min and Max in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-minimum-and-maximum-element-in-an-array4428/1)

### Problem Description

**Task:** Given an array arr[]. Your task is to find the minimum and maximum elements in the array.Examples:Input: arr[] = [1, 4, 3, 5, 8, 6]

#### Examples

##### Example 1

- **Output:**
```text
[3, 15]Explanation: minimum and maximum element of array are 3 and 15.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Java)

- **Submitted:** 2026-11-20 16:46:40
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public ArrayList<Integer> getMinMax(int[] arr) {
        int max = Integer.MIN_VALUE;
        int min = Integer.MAX_VALUE;
        
        for(int num : arr){
            if (num < min) 
            {min = num;}
            
            if (num > max){
                max = num;
            }
        }
        
        ArrayList<Integer> result = new ArrayList<>();
        result.add(min);
        result.add(max);
        return result;
        
        
    }
    
    public static void main(String[] args){
        int[] arr = {3,5,4,1,9};
       Solution obj = new Solution();
       ArrayList<Integer> result = obj.getMinMax(arr);
        System.out.println(result.get(0) + " " + result.get(1));
    }
    
    
}
```

#### Solution 2 (Java)

- **Submitted:** 2026-11-20 16:46:38
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public ArrayList<Integer> getMinMax(int[] arr) {
        int max = Integer.MIN_VALUE;
        int min = Integer.MAX_VALUE;
        
        for(int num : arr){
            if (num < min) 
            {min = num;}
            
            if (num > max){
                max = num;
            }
        }
        
        ArrayList<Integer> result = new ArrayList<>();
        result.add(min);
        result.add(max);
        return result;
        
        
    }
    
    public static void main(String[] args){
        int[] arr = {3,5,4,1,9};
       Solution obj = new Solution();
       ArrayList<Integer> result = obj.getMinMax(arr);
        System.out.println(result.get(0) + " " + result.get(1));
    }
    
    
}
```

*Generated on: 20/11/2026, 4:47:20 pm*