//print kth Smallest Ele 
import java.util.Stack;
class Node {
 
    int key;
    Node left, right;
    
    Node() {
       left = right = null; 
    }
 
    Node(int d) {
        key = d;
        left = right = null;
    }
}

class BinarySerachTree {
    
    static Node root;
    
    Node insert(Node node, int data) {
         
        /* 1. If the tree is empty, return a new,     
         single node */
        if (node == null) {
            return (new Node(data));
        } else {
             
            /* 2. Otherwise, recur down the tree */
            if (data <= node.key) {
                node.left = insert(node.left, data);
            } else {
                node.right = insert(node.right, data);
            }
 
            /* return the (unchanged) node pointer */
            return node;
        }
    }
    
    int kthSmallestEle(Node root, int k) { 
        
        if(root == null) {
            return 0;
        }
        
        Stack<Node> stack = new Stack<Node>();
        Node node = root;
        
        int ele = 0;
        
        while(node != null) {
            stack.push(node);
            node = node.left;
        }
        
        while(stack.size() > 0) {
            node = stack.pop();
            k--;
            if(k >= 0) {
                ele = node.key;
            }
            else {
                break;
            }
            
            if(node.right != null) {
                
                //node this branches left nodes
                node = node.right;
                while(node != null) {
                    stack.push(node);
                    node = node.left;
                }
            }
        }
        
        return ele;
    }
    
    
    void inOrderTraversal(Node root) { 
        
        if(root == null) {
            return;
        }
        
        Stack<Node> stack = new Stack<Node>();
        Node node = root;
        
        while(node != null) {
            stack.push(node);
            node = node.left;
        }
        
        while(stack.size() > 0) {
            node = stack.pop();
            System.out.println(node.key);
            
            
            if(node.right != null) {
                
                //node this branches left nodes
                node = node.right;
                while(node != null) {
                    stack.push(node);
                    node = node.left;
                }
            }
        }
        
    }
    
    
     public static void main(String[] args) {
        /* Following BST
              20
           /     \
          8      22
         /  \    
       4    12  
            / \
           10  14
       */
        BinarySerachTree tree = new BinarySerachTree();
        Node root = null;
        root = tree.insert(root, 20);
        root = tree.insert(root, 8);
        root = tree.insert(root, 22);
        root = tree.insert(root, 4);
        root = tree.insert(root, 12);
        root = tree.insert(root, 10);
        root = tree.insert(root, 14);
 
        //output = 12
        System.out.println("kth Smallest: " + tree.kthSmallestEle(root, 4));
    
    }
}
