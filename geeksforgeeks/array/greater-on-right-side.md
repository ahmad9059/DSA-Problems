## Problem Code
```cpp
class Solution{
public:	
	/* Function to replace every element with the
	next greatest element */
	void nextGreatest(int arr[], int n) {
	    // code here
	    int temp,mfr=-1;
	    for(int i=n-1;i>=0;i--)
	    {
	        temp=arr[i];
	        arr[i]=mfr;
	        mfr=max(temp,mfr);
	    }
	}

};
