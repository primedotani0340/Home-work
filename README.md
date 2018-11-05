# Home-work
NAME=muhammad Idrees Roll No# 34
#include <iostream>
#include <conio.h>
using namespace std;
int main()
{
int a[12]={7,9,11,13,23,27,28,37,41,47,53,57};
    int i,count,n,l,r,m;
    count=12;
for (i=0; i<count; i++)
{
}
cout<<"Enter the number that you want to search:"; 
        cin>>n;
l = 0;
r = count-1;
m = (l+r)/2;
while (l <= r)
{
   if(a[m] < n)
   {
l = m + 1;

   }
   else if(a[m] == n)
   {
cout<<n<<" found in the array at the location "<<m<<"\n"; 
                break; 
           } 
           else { 
                r = m - 1; 
           } 
           m = (l + r)/2; 
        } 
        if(l > r)
{
   cout<<n<<" not found in the array";
}
return 0;
}
