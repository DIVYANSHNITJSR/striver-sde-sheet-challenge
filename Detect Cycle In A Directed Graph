#include<bits/stdc++.h>


int detectCycleInDirectedGraph(int n, vector < pair < int, int >> & edges) {
  
 vector<int>adj[n+1];
 
 int k=edges.size();
for(int i=0;i<k;i++){
  int u=edges[i].first;
  int v=edges[i].second;

  adj[u].push_back(v);

}


int indegree[n+1]={0};

for(int i=1;i<=n;i++){
  for(auto x:adj[i]){
      indegree[x]++;
  }
}

 int cnt=0;
 queue<int>q;

for(int i=1;i<=n;i++){
  if(indegree[i]==0){
    q.push(i);
  }
}

while(!q.empty()){
  int node=q.front();
      q.pop();
      cnt++;
 for(auto x: adj[node]){
   indegree[x]--;
   if(indegree[x]==0){
     q.push(x);
   }
  }
      
}

  if(cnt==n)
     return false;

  return true;


}
