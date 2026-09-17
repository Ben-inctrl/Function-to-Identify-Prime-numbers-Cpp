# Function-to-Identify-Prime-numbers-Cpp
A program that checks whether a number entered is a prime number.

#include <iostream>
using namespace std;

bool primeNum(int num);

int main(){
    int num;
    cout<<"Enter a number:\n";
    cin>>num;
    if(primeNum(num)){
        cout<<"true\n";
    }
    else{
        cout<<"false\n";
    }
    return 0;
}

bool primeNum(int num){
    if(num<=1)
    return false;
    
    for( int i=2 ; i<=num/2 ; i++){
        if(num%i==0)
        return false;
    }
    return true;
}

