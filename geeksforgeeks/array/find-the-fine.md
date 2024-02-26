## Problem Code
```cpp
class Solution{
  public:
    long long int totalFine(int n, int date, int car[], int fine[])
    {
        long long ans=0;
        for(int i=0;i<n;i++)
        {
            if(date%2==0)
            {
                if(car[i]%2!=0)
                ans+=fine[i];
            }
            else
            {
                if(car[i]%2==0)
                ans+=fine[i];
            }
        }
        return ans;
    }
};
```
