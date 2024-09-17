//# Minimum-and-Maximum-in-2-D-Array
#include<iostream>
#include<limits.h>
using namespace std;
void minimum(int a[][4],int rownumber,int colnumber){
    int min = INT_MAX;
    int i,j;
    for(i=0;i<rownumber;i++){
        for(j=0;j<colnumber;j++){
            if(min>a[i][j]) min = a[i][j];
        }
    }
    cout<<"Minimum Element : "<<min;
}
void maximum(int a[][4],int rownumber,int colnumber){
    int max = INT_MIN;
    int i,j;
    for(i=0;i<rownumber;i++){
        for(j=0;j<colnumber;j++){
            if(max<a[i][j]) max = a[i][j];
        }
    }
    cout<<"Maximum Element : "<<max;
}
int main(){
    int a[3][4];
    int rownumber = 3;
    int colnumber = 4;
    int i,j;
    cout<<"Enter Array Element"<<endl;
    for(i=0;i<rownumber;i++){
        for(j=0;j<colnumber;j++){
            cin>>a[i][j];
        }
    }
    // minimum(a,rownumber,colnumber);
    maximum(a,rownumber,colnumber);
}
