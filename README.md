// decimal-to-binary-octal
// for decimal to binary --> num = 2
// for decimal to octal --> num = 8
#include <iostream>

using namespace std;

int binary(int n){
    int temp,bin=0,c=1,num=2;
    while(n!=0){
        temp=n%num;
        bin=bin+temp*c;
        n=n/num;
        c*=10;
    }
    return bin;
}

int main()
{
    int n;
    cout<<"enter the number: ";
    cin>>n;
    cout<<binary(n);

    return 0;
}
