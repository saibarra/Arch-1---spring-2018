#include <stdio.h>
#include <stdlib.h>

struct node{
  int value;
  struct node *left, *right;
};


struct node *newNode(int value){
  struct node *temp = (struct node*)malloc(sizeof(struct node));
  temp->value = value;
  temp->left = temp->right = NULL;
  return temp;
}


void inorder(struct node *root){
  if(root != NULL){
    inorder(root->left);
    printf("%d \n", root->value);
    inorder(root->right);
  }
}


struct node* insert(struct node* node, int value){
  if(node == NULL)
    return newNode(value);

  if(value < node->value)
    node->left = insert(node->left, value);
  else if(value > node->value)
    node->right = insert(node->right, value);

  return node;
}


int main(){
  struct node *root = NULL;
  root = insert(root, 50);
  insert(root, 60);
  insert(root, 30);
  insert(root, 80);
  insert(root, 90);
  insert(root, 20);
  insert(root, 10);
  insert(root, 50);
  insert(root, 40);
  insert(root, 70);

  inorder(root);
  return 0;
}
