# Valera Chichkin
### > [Junior Frontend Developer](https://pplays33.github.io/rsschool-cv/cv)

***

## Contact info
#### email: pplayps98@gmail.com
#### discord-rs: vaime(@pplays33)
#### [github](https://github.com/Vaiem)
***

## About Myself

My goal is to develop in the field of Frontend development and create high-quality and user-friendly interfaces for users. The main priority for me is continuous professional development and improvement of my skills.

My strengths:

* Excellent knowledge of HTML/CSS and JavaScript
* Good understanding of UX/UI design principles
* Basic knowledge of c++, Rust.
* Knowledge of Python (django, flask, matplotlib...)
* Ability to work with Git and other development tools

* Knowledge of Algorithms(Hoffman, trees, garfs, workarounds...)

I have worked on several projects, including building websites and web applications. In particular, I did django layout and backend development: https://github.com/Vaiem/FastExchange , which gave me experience with Django, bootstrap, pip. 

I also built a mini web framework in Rust: https://github.com/Vaiem/LibFFW , I used cargo, tokio and wrote macros for it.

If we talk about my aspirations, I always try to learn something new and apply it to my work. To do this, I attend online courses, watch video lessons and read articles about new technologies and tools.

I believe that my knowledge, experience, and desire to improve will allow me to become a valuable member of the Frontend development team.

***

## Skills and Proficiency:

* HTML5, CSS3
* JavaScript, python
* Git, GitHub
* VS Code, WebStorm
* figma
* leetcode

![](https://leetcode.com/static/images/badges/2022/gif/2022-annual-50.gif) 

***

## > Code example:

### BinarySearchTreeIterator

### LeetCode-173

Implement the BSTIterator class that represents an iterator over the in-order traversal of a binary search tree (BST):
BSTIterator(TreeNode root) Initializes an object of the BSTIterator class. The root of the BST is given as part of the constructor. The pointer should be initialized to a non-existent number smaller than any element in the BST.
boolean hasNext() Returns true if there exists a number in the traversal to the right of the pointer, otherwise returns false.
int next() Moves the pointer to the right, then returns the number at the pointer.
Notice that by initializing the pointer to a non-existent smallest number, the first call to next() will return the smallest element in the BST.

You may assume that next() calls will always be valid. That is, there will be at least a next number in the in-order traversal when next() is called.

``` c++

    /**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode *left;
 *     TreeNode *right;
 *     TreeNode() : val(0), left(nullptr), right(nullptr) {}
 *     TreeNode(int x) : val(x), left(nullptr), right(nullptr) {}
 *     TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {}
 * };
 */
class BSTIterator {
    TreeNode* currentNode = nullptr;
public:
    BSTIterator(TreeNode* root) {
       recTree(root);
    }
    
    int next() {
        if(currentNode != nullptr)
        {   
            int item = currentNode->val;
            currentNode = currentNode->right;
            return item;
        }
        return INT_MIN;
    }
    
    bool hasNext() {
        if(currentNode != nullptr)
        {
            return true;
        }
        return false;
    }

    void recTree(TreeNode* root)
    {
        if(root == nullptr)
        {
          return;
        }

        recTree(root->right);
        root->right = currentNode;
        currentNode = root;

        recTree(root->left);

    }
};

/**
 * Your BSTIterator object will be instantiated and called as such:
 * BSTIterator* obj = new BSTIterator(root);
 * int param_1 = obj->next();
 * bool param_2 = obj->hasNext();
 */

```
***

## Courses:
* RS Schools Course «JavaScript/Front-end. Stage 0» (in progress)

***

## Languages:
* English - Elementary/Intermediate 
* Russia: native

