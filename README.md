# Experiment---17 

### Aim 
To study and implement Linked List in C++. 

### Software 
Visual Studio Code 

### Theory 
A linked list is a fundamental data structure. It mainly allows efficient insertion and deletion operations compared to arrays. Like arrays, it is also used to implement other data structures like stack, queue and deque. <br> 

<b>Comparison of Linked List and Arrays</b> 

<ul><li>Linked List:</li>
<ol><li>Data Structure: Non-contiguous</li>
<li>Memory Allocation: Typically allocated one by one to individual elements</li>
<li>Insertion/Deletion: Efficient</li>
<li>Access: Sequential</li>
<li>Array:</li></ul>
<li>Data Structure: Contiguous</li>
<li>Memory Allocation: Typically allocated to the whole array</li>
<li>Insertion/Deletion: Inefficient</li>
<li>Access: Random</li></ol>
 
### Code       
(A) <br> 
```
// NAME - SHLOKA PATEL 
// PRN - 23070123120 
// EXPERIMENT - 17 

// LINKED LIST 

#include<iostream>
using namespace std; 
 
 class Link {
    public:
    int data;
    Link* next;
    Link(int num) {
        data=num;
        next=NULL;
    }
 };
 void insert_head(Link* &head, int data) {
    Link* new_node=new Link(data);
    new_node->next = head; 
    head = new_node;
 }
 void disp(Link* head) {
    Link* temp = head;
    while(temp!=NULL) { 
        cout<<temp->data<<"->";
        temp = temp->next;
    } 
    cout<<"NULL"<<endl;
 }

 int main() {
    Link* head = NULL;
    insert_head(head, 30);
    disp(head);
    insert_head(head, 32);
    disp(head);
    insert_head(head, 35);
    disp(head);
    //l1.disp(); 
 }  
```

### Output 
(A) <br> 
![](https://github.com/Shloka-Patel/Experiment---17/blob/main/Output_17A.png) 

### Conclusion 
