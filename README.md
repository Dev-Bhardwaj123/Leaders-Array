# Leaders-Array
Find leader elements in the array i.e no element on right must be greater than the current element
//Leaders in array (no element on right must be greater)
#include<iostream>
#include<bits/stdc++.h>
using namespace std;

int main(){
	int n;
	cout<<"Enter size: ";
	cin>>n;
	int arr[n];
	for(int i=0;i<n;i++){
		cin>>arr[i];
	}
	int curr=arr[n-1];
	cout<<curr<<" ";
	for(int i=n-2;i>=0;i--){
		if(curr<arr[i]){
			curr=arr[i];
			cout<<curr<<" ";
		}
	}
	return 0;
}
