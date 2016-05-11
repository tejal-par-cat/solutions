//InOrderSuccessor : is the next node which appears in Inorder traversal of BST
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

class Result {
    Node pre;
    Node succ;
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
    
    
    Result findSucc(Node root, Result result, int key) {
        if(root == null) {
            return result;
        }
        
        if(root.key == key) {
            
            if(root.right != null) {
                Node temp = root.right;
                
                while(temp.left != null) {
                    temp = temp.left;
                }
                
                result.succ = temp;
            }
        }
        
        if(root.key > key) {
            //succ is current node
            
            result.succ = root;
            result = findSucc(root.left, result, key);
        }
        else {
            result = findSucc(root.right, result, key);
        }
        
        return result;
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
 
        Result result = new Result();
        result = tree.findSucc(root, result, 10);
        
        if(result.succ != null) {
            System.out.println("o/p Succ: " + result.succ.key);
        }
    }
}

//succ of 8 is 10, 10 is 12 and 14 is 20
