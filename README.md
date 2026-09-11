#include<bits/stdc++.h>
using namespace std;
int main(){
     int n ;
    cout<<"Enter size of array";
    cin>>n;
    int arr[n];
     for(int i=0;i<n;i++){
         cin>>arr[i];
         
     }
    int k=0;
    
    int temp;// Selection sort 
     int max;
    

    for(int i=0;i<n;i++){
         max=arr[i];
        for(int j=i;j<n;j++){
            if(arr[j]<max){
                max=arr[j];
                k=j;
                
                    
            }
            
        }
       
      
        
        temp=arr[i];
        arr[i]=arr[k];
        arr[k]=temp;
        
        
    }
     for(int i=0;i<n;i++){
         cout<<arr[i]<<endl;
         
     }
       

    
}


