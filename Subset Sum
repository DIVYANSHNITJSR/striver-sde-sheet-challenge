#include <bits/stdc++.h> 

void f(int ind,vector<int>&num,int n ,int sum,vector<int>&ans)

{

    if(ind==n)

    {

        ans.push_back(sum);

        return ;

    }

    f(ind+1,num,n,sum+num[ind],ans);

    f(ind+1,num,n,sum,ans);

}

 

vector<int> subsetSum(vector<int> &num)

{

    // Write your code here.

    vector<int>ans;

    int n=num.size();

    f(0,num,n,0,ans);

    sort(ans.begin(),ans.end());

    return ans;

 

}
