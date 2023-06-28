/* The Node structure is
struct Node
{
    int data;
    Node* left;
    Node* right;
}; */

class Solution{
  public:
    /*You are required to complete this method*/
    int maxDepth(Node *root) {
        // Your code here
        if(root == NULL) return 0;
        return max(1+maxDepth(root->left), 1+maxDepth(root->right));
    }
};
