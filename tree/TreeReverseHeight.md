# Binary Tree Reverse Height (Postorder Height Calculation)

## 📌 Problem Statement

Given the root of a binary tree, compute and print the **height of each node** using **postorder traversal (Left → Right → Root)**.

### Height Definition

- Height of a node = number of **edges** in the longest path from that node to a leaf.
- Height of a leaf node = `0`
- Height of a null node = `-1`

For each node, print:

```
nodeValue->height
```

The function should also return the height of the root.

---

## 🌳 Example Tree Used in This Program

The `main` method constructs the following binary tree:

```
        1
       / \
      2   3
     / \
    4   5
```

---

## ✅ Expected Output

### Inorder Traversal Output (printTree)

```
4
2
5
1
3
```

### Reverse Height Output (Postorder)

```
4->0
5->0
2->1
3->0
1->2
```

### Root Height Returned

```
2
```

---

## 🧠 Approach

The algorithm uses **recursion** with postorder traversal:

1. Recursively compute left subtree height.
2. Recursively compute right subtree height.
3. Compute current node height:

   ```
   height = 1 + max(leftHeight, rightHeight)
   ```

4. Print the node value and height.
5. Return height.

### ⏱ Time Complexity

```
O(n)
```

Each node is visited once.

### 🗂 Space Complexity

```
O(h)
```

Where `h` is the height of the tree (recursion stack).

---

## 💻 Full Java Implementation

```java
class TreeReverseHeight {
    public static void main(String[] args) {
        TreeNode root = new TreeNode(1);

        TreeNode t = new TreeNode(2);
        root.left = t;

        t = new TreeNode(3);
        root.right = t;

        t = new TreeNode(4);
        root.left.left = t;

        t = new TreeNode(5);
        root.left.right = t;

        TreeOp treeOp = new TreeOp();

        System.out.println("Inorder Traversal:");
        treeOp.printTree(root);

        System.out.println("\nReverse Height (Postorder):");
        int height = treeOp.printTreeReverseHeight(root);

        System.out.println("\nRoot Height: " + height);
    }
}

class TreeOp {

    // Prints height of each node using postorder traversal
    public int printTreeReverseHeight(TreeNode root) {
        if (root == null) return -1;

        int leftH = printTreeReverseHeight(root.left);
        int rightH = printTreeReverseHeight(root.right);

        int height = 1 + Math.max(leftH, rightH);

        System.out.println(root.val + "->" + height);

        return height;
    }

    // Inorder traversal
    public void printTree(TreeNode root) {
        if (root == null) return;

        printTree(root.left);
        System.out.println(root.val);
        printTree(root.right);
    }
}

class TreeNode {
    int val;
    TreeNode left;
    TreeNode right;

    public TreeNode(int val) {
        this.val = val;
        this.left = null;
        this.right = null;
    }
}
```

---

## 🔎 Key Takeaways

- Demonstrates **postorder traversal**
- Calculates height using **edge count definition**
- Clean recursive solution
- Suitable for interview preparation
