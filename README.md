# C-Linear-Search

#include <bits/stdc++.h>
using namespace std;

int linearSearch(int *arr,int n, int key){
    for(int i=0;i<n;++i){
        if(*(arr+i)==key){
            return i;
        }
    }
    return -1;
}
int main(){
    int n;
    cout<<"Enter length of array: ";
    cin>>n;
    int arr[n];
    cout<<"Enter elements of array: ";
    for(int i=0;i<n;++i){
        cin>>arr[i];
    }
    int key;
    cout<<"Enter key: ";
    cin>>key;
    cout<<linearSearch(arr,n,key);
}
