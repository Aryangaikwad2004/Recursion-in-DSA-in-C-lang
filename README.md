# Recursion-in-DSA-in-C-lang
#90days 
Some of the youtube tutorial codes of recursion 

#include<iostream>
using namespace std;

int Sum(int n){
    if(n==0){
        return 0;
    }
    int prevSum = Sum(n-1);
    return n + prevSum;

}

int main(){
int n;
cin>>n;

cout<<Sum(n)<<endl; 
return 0;
}



2.PROBLEM

#include <iostream>
using namespace std;

int power(int n, int p)
{

    if (p == 0)
    {
        return 1;
    }

    int prevPower = power(n, p - 1);
    return n * prevPower;
}
int main()
{
    int n, p;
    cin >> n >> p;
    cout << power(n, p) << endl;
    return 0;
}
