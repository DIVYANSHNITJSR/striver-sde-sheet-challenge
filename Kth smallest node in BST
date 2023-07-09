#include <bits/stdc++.h> 

void solve(TreeNode<int> *root, int k,priority_queue<int>&q){
    if(!root){
        return;
    }
    if(q.size()==k){
        if(q.top()>root->data){
            q.pop();
            q.push(root->data);
        }
    }
    else{
        q.push(root->data);
    }
    if(root->left){
        solve(root->left,k,q);
    }
    if(root->right){
        solve(root->right,k,q);
    }
}
int kthSmallest(TreeNode<int> *root, int k)
{
	//	Write the code here.
    priority_queue<int>q;
    solve(root,k,q);
    return q.top(); 
}
