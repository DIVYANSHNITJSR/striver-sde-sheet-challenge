#include <bits/stdc++.h> 
vector<int> topologicalSort(vector<vector<int>> &edges, int v, int e)  {
      
      int n=edges.size();
      vector<int>adj[v];
     for(int i=0;i<n;i++){
         int u=edges[i][0];
         int V=edges[i][1];

         adj[u].push_back(V);
     }
    
    int indegree[v]={0};

  for(int i=0;i<v;i++){    
       for(auto x:adj[i]){
            indegree[x]++;
       }
  }


  vector<int>ans;
   queue<int>q;
   for(int i=0;i<v;i++){
       if(indegree[i]==0){
           q.push(i);
       }
   }


   while(!q.empty()){
       int node=q.front();
       q.pop();
       ans.push_back(node);

       for(auto x:adj[node]){
           indegree[x]--;
           if(indegree[x]==0){
               q.push(x);
           }  
       }
   }


    return ans;

}
