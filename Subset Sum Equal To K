#include <bits/stdc++.h>

 

bool solve(int n, int k, vector<int> &arr, int index, vector<vector<int>> &dp){

 

if(k==0) return true;

if(index==n) return false;

 

if(dp[index][k]!=-1) return dp[index][k];

bool ans1= solve(n, k, arr, index+1, dp);

bool ans2= 0;

if(k-arr[index]>=0){

ans2= solve(n, k-arr[index], arr, index+1, dp);

}

 

return dp[index][k]= (ans1 || ans2);

}

bool subsetSumToK(int n, int k, vector<int> &arr) {

vector<vector<int>> dp(n,vector<int>(k+1, -1));

return solve(n, k, arr, 0, dp);

}
