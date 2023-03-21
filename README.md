#include<iostream>  
using namespace std;  
   
int main(){  
    int n; //聲明n這個變量 
    cin>>n; //讀取輸入的值，將其存到n中 
    while (n--) //n大於0時，會執行迴圈，每次執行n-1 
    {  
        int a1,a2,b1,b2; //定義了四個整數變數，名稱為a1、a2、b1和b2 
        char w; 宣告了一個名稱為w的變數 
        cin>>w>>a1>>a2>>b1>>b2; //從輸入裝置讀入數據，並將其儲存在不同的變數中 
        switch(w){ //根據w的值，從以下case標籤中選擇一個來執行 
            case '+':cout<<a1+b1<<" "<<a2+b2<<"\n";break;  
            case '-':cout<<a1-b1<<" "<<a2-b2<<"\n";break;  
            case '*':cout<<a1*b1-a2*b2<<" "<<a2*b1+a1*b2<<"\n";break;  
            case '/':cout<<(a1*b1+a2*b2)/(b1*b1+b2*b2)<<" "<<(a2*b1-a1*b2)/(b1*b1+b2*b2)<<"\n";break;  
        }  
    }  
       
} 
