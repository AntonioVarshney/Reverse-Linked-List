//Reverse-Linked-List
//Reverse Linked List by iterative method

#include<bits/stdc++.h>
using namespace std;

void reverse()
{
  Node* prev = NULL;
  Node* next = NULL;
  Node* curr;
  while(curr!=NULL)
  {
    next = curr->next;
    curr->next = prev;
    prev = curr;
    curr = next;
  }
}
int main()
{
  reverse();
  return 0;
} 
