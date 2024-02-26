## Problem Code
```
class Solution {
  public:
    int missingNumber(int n, vector<int> &arr) {
        // code here
        long long sum=0;
        long long num=(n*(n+1))/2;
        for(int i=0;i<n-1;i++)
        {
            sum+=arr[i];
        }
        return num-sum;
    }
};
```
