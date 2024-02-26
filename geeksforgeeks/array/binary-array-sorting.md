## Problem Code
```cpp
class Solution{
  public:
    
    // A[]: input array
    // N: input array
    //Function to sort the binary array.
    void binSort(int arr[], int N)
    {
       //Your code here
       int num=0;
        for(int i=0;i<N;i++)
        {
            num+=arr[i];
        }
        int zero;
        zero=N-num;
        for(int i=0;i<zero;i++)
        arr[i]=0;
        for(int i=zero;i<N;i++)
        arr[i]=1;
        
    }

};
```
