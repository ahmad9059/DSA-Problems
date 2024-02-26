## Problem code
```cpp
//User function template for C++

class Solution{   
public:
    int findMissing(int arr[], int n) {
        // code here
        int diff= (arr[n-1]-arr[0])/n;
        for(int i=0;i<n;i++)
        {
            if(arr[i+1]-arr[i]!=diff)
            {
                return arr[i]+diff;
            }
        }
        
}
};
```
