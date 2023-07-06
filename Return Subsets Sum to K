#include <bits/stdc++.h>

 

void rec(int ind, vector<int>& arr, int k, vector<vector<int>>& ans, vector<int>& ds){

if(ind == arr.size()){

if(accumulate(ds.begin(), ds.end(), 0) == k){

ans.push_back(ds);

}

return;

}

 

ds.push_back(arr[ind]);

rec(ind + 1, arr, k, ans, ds);

ds.pop_back();

rec(ind + 1, arr, k, ans, ds);

}

 

vector<vector<int>> findSubsetsThatSumToK(vector<int> arr, int n, int k)

{

vector<vector<int>> ans;

vector<int> ds;

 

rec(0, arr, k, ans, ds);

 

return ans;

}
