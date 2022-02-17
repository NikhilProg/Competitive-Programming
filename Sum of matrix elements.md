#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;
typedef long long l1;


int main() {
    int t;
    cin>>t;
    while(t--){
        l1 n;
        cin>>n;
        l1 res=0;
        for(l1 i=0 ; i<n ; i++){
            for(l1 j=0 ; j<n ; j++){
                l1 x;
                cin>>x;
                if(i==0||j==0||i==n-1||j==n-1||i==j||i+j==n-1){
                    res+=x;
                }
            }
        }
        cout<<res<<"\n";
    }
    return 0;
}
