# Prime-Number-C-
//*Find the prime number in c++ code.*//
#include<iostream>
#include<conio.h>

using namespace std;

int main()
{
    int n,i,flag , c=0;
    cout<<"Prime number from 1 to 100 are:-> ";
    for (n=1; n<=100; n++)
    {
        flag=0;
        for (i=2; i<=n/2; i++)
        {
            if(n%i==0)
            {
                flag=1;
                break;

            }
        }
        if(flag==0&&n!=1 )
        {
            cout<<n<<",";
            c++;

        }
    }
    cout<<"\ntotal prime = "<<c;
    getch();

}
