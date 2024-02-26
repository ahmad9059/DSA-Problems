## Problem Code
```cpp
class Solution
{
    public:
    //rotate string clockwise
    string rotateclockwise(string s)
    {
        char ch =s[s.size()-1];
        int index=s.size()-2;
        while(index>=0)
        {
            s[index+1]=s[index];
            index--;
        }
        s[0]=ch;
        return s;
    }
    string rotateclockantiwise(string s)
    {
        char ch = s[0];
        int index=0;
        while(index<s.size()-1)
        {
            s[index]=s[index+1];
            index++;
        }
        s[s.size()-1]=ch;
        
        return s;
    }
    bool isRotated(string str1, string str2)
    {
        string s1,s2;
        s1=rotateclockwise(str1);
        s1=rotateclockwise(s1);
        if(s1==str2)
        return 1;
        s2=rotateclockantiwise(str1);
        s2=rotateclockantiwise(s2);
        if(s2==str2)
        return 1;
        
        
    return 0;
        
    }

};
```
