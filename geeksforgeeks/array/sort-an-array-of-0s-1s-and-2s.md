## Problem Code - Sort an array of 0s, 1s and 2s
```cpp
class Solution
{
    public:
    void sort012(int arr[], int n)
    {
        // code here
        long long zero=0,one=0;
        for(int i=0;i<n;i++)
        {
            if(arr[i]==0)      zero++;
            else if(arr[i]==1) one++;
        }
        for(int i=0;i<zero;i++)        arr[i]=0;
        for(int i=zero;i<zero+one;i++) arr[i]=1;
        for(int i=zero+one;i<n;i++)    arr[i]=2;
        
        
    }
    
};
```
