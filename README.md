#include <iostream>
using namespace std;
int main(){
    int n;
    cin>>n;
    int arr[n];
    for(int i=0;i<n;i++){
        cin>>arr[i];
    }
    int target;
    cin>>target;
    int count =0;
    for(int i=0;i<n-1;i++){
        for(int j=i+1;j<n;j++){
            if(target==arr[i]+arr[j]){
                count =1;
                break;
            }
        }
    }
    if(count ==1){
        cout<<"yes";
    }
    else{
        cout<<"No";
    }
}
