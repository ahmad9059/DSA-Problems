## Problem Code
```cpp
class Solution
{
    public:
    //Function to find a continuous sub-array which adds up to a given number.
    vector<int> subarraySum(vector<int>arr, int n, long long s)
    {
        // Your code here
        int start=0,sum=0;
        for(int i=0;i<n;i++)
        {
            sum+=arr[i];
            while(sum>s && start<i)
            {
                sum-=arr[start];
                start++;
            }
            if(sum==s)
            return {start+1,i+1};
        }
        return {-1};
    }
};
```
