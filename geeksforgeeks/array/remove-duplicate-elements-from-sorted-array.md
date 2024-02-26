## Problem Code
### My logic
```cpp
//User function template for C++

class Solution{
public:
    int remove_duplicate(int a[],int n){
        // code here
        vector<int>unique;
        int temp=-1,count=0;
        for(int i=0;i<n;i++)
        {
            if(a[i]!=temp)
            {
                unique.push_back(a[i]);
                count++;
                temp=a[i];
            }
        }
        for(int i=0;i<n;i++)
        {
            a[i]=unique[i];
        }
        return count;
        
    }
};
```
### Better Logic
```cpp
class Solution{
public:
    int remove_duplicate(int a[],int n){
        // code here
        int i=0;
        for(int j=1;j<n;j++)
        {
            
            if(a[i]!=a[j])
            {
            i++;
            a[i]=a[j];
            }
        }
        return i+1;
    }
};
```
