## Problem Code
```
class Solution{
    public:
    void segregateElements(int arr[],int n)
    {
        // Your code goes here
        int j=0;
        vector<int>ans;
        //for positive values
        for(int i=0;i<n;i++)
        {
            if(arr[i]>=0)
            {
                ans.push_back(arr[i]);
                j++;
            }
        }
        //for negative values
        for(int i=0;i<n;i++)
        {
            if(arr[i]<0)
            {
                ans.push_back(arr[i]);
                j++;
            }
        }
        for(int i=0;i<n;i++)
        {
            arr[i]=ans[i];
        }
        
    }
};
```
