# program-to-search-for-an-element-using-linear-search.

#include<iostream>
    using namespace std;
    int main(){
        int n;
        cout<<"enter the size of array";
        cin>>n;

        int arr[n];
        for(int i=0;i<n;i++){
        cout<<"enter the elements of array "<<i+1<<" ";
        cin>>arr[i];
        }   

        int key;
        int found=0;

        cout<<"enter elements to search ";
        cin>>key;
        
        for(int i=0;i<n;i++){
            if(arr[i]==key){
                cout<<"element has found "<<i;
                found=1;
                break;
            }
        }
        if(found==0){
            cout<<"element has not found";
        }
        return 0;
    }
