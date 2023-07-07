#include <bits/stdc++.h> 

class Queue {

    // Define the data members(if any) here.

    stack<int> s1;

    stack<int> s2;

    stack<int> s3;

    int size;

    public:

   Queue() {

        // Initialize your data structure here.

        size=0; 

   }

   void enQueue(int val) { 

       // Implement the enqueue() function.

        s2.push(val);

        while(!s1.empty()){ 

           s3.push(s1.top()); 

           s1.pop(); 

       }

        while(!s3.empty()){

            s2.push(s3.top());

            s3.pop(); 

       }

        size++;

        swap(s1,s2);

        return;

   }

 

   int deQueue() { 

       // Implement the dequeue() function.

        if(size<=0){ 

           return -1;

        } 

       else{ 

           int ans=s1.top();

            s1.pop(); 

           size--; 

           return ans; 

       }

    }

   int peek() { 

       if(size<=0){

            return -1;

        }

        return s1.top();

    }

 

   bool isEmpty() { 

       // Implement the isEmpty() function here. 

       return !size;

    }

 };
