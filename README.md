# calendar
//This code was created in C++ and it's purpose is to practive if statements and do while loops. The user enters a date and the program will determine if the date entered is a valid date. 

#include<iostream>
using namespace std;

int main ()
{
 int m,d,y;
char sign;
do 
{
cout<<"enter a valid date"<<endl; 
cin>>m>>sign>>d>>sign>>y;
if(m)
{
  if(m >=1 && m<=12)
  {
    cout<<"month is valid"<<endl;
  }
  if (m<1)
  {
    cout<<"Month is invalid setting it to January 1, 2000"<<endl;
     m=1; 
     d=1;
     y=2000;
    cout<<m<<"/"<<d<<"/"<<y;
  }
}

if(d)
{
   if(d>=1 && d<=31)
    { 
      cout<<"valid day"<<endl;
    }
   if(d<1 || d > 31)
    {
      cout<<"Month is invalid setting it to January 1, 2000"<<endl;
     m=1; 
     d=1;
     y=2000;
    cout<<m<<"/"<<d<<"/"<<y;
    }
}

if(y)
{
  if(y>0)
   {
    cout<<"Valid Year"<<endl;
   }
  if(y<0)
   {
     cout<<"Month is invalid setting it to January 1, 2000"<<endl;
     m=1; 
     d=1;
     y=2000;
    cout<<m<<"/"<<d<<"/"<<y;
 
   }
}
}while(y>0);



return 0;
}
