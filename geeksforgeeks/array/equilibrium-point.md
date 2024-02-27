### Problem Code - Equilibrium Point
```cpp
class Solution{
    public:
    // Function to find equilibrium point in the array.
    // a: input array
    // n: size of array
    int equilibriumPoint(long long a[], int n) {
    
        // Your code here
        int totalSum=0,leftSum=0;
        for(int i=0;i<n;i++){
            totalSum+=a[i];
        }
        for(int i=0;i<n;i++){
            totalSum-=a[i];
            if(totalSum==leftSum)
            return i+1;
            leftSum+=a[i];
        }
        return -1;
    }

};
```
