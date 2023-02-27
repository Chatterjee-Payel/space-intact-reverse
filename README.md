# space-intact-reverse
class Solution
{
  public:
  
        string reverseWithSpacesIntact (string s)
        {
            //code here.
          int l=0,r=s.size()-1;
          while(l<r)
          {
              if(s[l]==' '){
                  l++;
              }
              else if(s[r]==' '){
              r--;
          }
          else{
              swap(s[l],s[r]);
              l++;
              r--;
          }
        }
        
          return s;
        }
        
};
