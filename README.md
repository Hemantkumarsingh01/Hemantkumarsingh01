#include<bits/stdc++.h>
using namespace std;

int factorial(int n){
    int facto=1;
    for(int i=1;i<n;i++){
        facto  = facto*i;
    }
    return facto;
}
int nCr(int n,int r){
    int a=factorial( n);
    int b=factorial( r) * factorial(n-r);
    return a/b;
}
int main(){
    int n,r;
    cout<<"enter the no n :";
    cin>>n;
    cout<<"enter the no r :";
    cin>>r;
    cout<<"the ans is:" <<nCr(n,r);
    return 0;
}
