Download Link: https://assignmentchef.com/product/solved-comp-2000-assignment-2
<br>
<ol>

 <li><strong> Part 1</strong>Binary search tree</li>

</ol>




A node of a binary search tree (BST) of integers is defined as




typedef struct {    int    data;    struct Node* left;    struct Node* right;

} Node;




A binary search tree <strong>root</strong> is declared by




treePtr root = NULL;




where treePtr is defined as below.




typedef Node* treePtr;




Write a complete program <strong>BST.c</strong> to demonstrate basic operations on a binary search tree of integers. Your program should show the following options.




<ol>

 <li>Insert a new node (iteration)</li>

 <li>Insert a new node (recursion)</li>

 <li>Tree traversal</li>

 <li>Search a node (iteration)</li>

 <li>Search a node (recursion)</li>

 <li>Count number of nodes in tree</li>

 <li>Count number of leaves in tree</li>

 <li>Height of tree (root level = 0)</li>

 <li>Height of tree (root level = 1)</li>

 <li>Find the node with minimum key (iteration)</li>

 <li>Find the node with minimum key (recursion)</li>

 <li>Find the node with maximum key (iteration)</li>

 <li>Find the node with maximum key (recursion)</li>

 <li>Delete a node from BST (iteration)</li>

 <li>Delete a node from BST (recursion)</li>

 <li>Find the inorder successor (without using parent link)</li>

 <li>Breadth-first traversal (BFT)</li>

 <li>Exit</li>

</ol>

Select your choice (1-18):




The program allows a user to choose one of the above options by entering an integer from 1 to 18 to perform the corresponding action.

The marks are given as follows.




<ol>

 <li>Insert a new node (iteration). The <strong>insert()</strong> function allows the user to iteratively insert a new element into the BST.</li>

 <li>Insert a new node (recursion). The <strong>insertR()</strong> function allows the user to recursively add a new element into the BST.</li>

 <li>Tree traversal. This option allows the user to select the inorder, preorder, or postorder traversal by entering an integer 1, 2, or 3, respectively, to perform the corresponding action.</li>

 <li>Search a node (iteration). The <strong>search()</strong> function iteratively searches on the BST for the specified search key <strong>x</strong>, where <strong>x</strong> is input by the user. The <strong>search()</strong> function returns the node containing <strong>x</strong> if it is found; otherwise <strong>NULL</strong> is returned.</li>

 <li> Search a node (recursion). The <strong>searchR()</strong> function recursively searches on the BST for the specified search key <strong>x</strong>, where <strong>x</strong> is entered by the user. The <strong>searchR()</strong> function returns the node containing <strong>x</strong> if it is found; otherwise <strong>NULL</strong> is returned.</li>

 <li> Count number of nodes in tree. The <strong>countNodes()</strong> function returns the number of nodes in the BST.</li>

 <li>Count number of leaves in tree. The <strong>countLeaves()</strong> function returns the number of leaf nodes in the BST.</li>

 <li> Height of tree (root level = 0). The <strong>compHeight()</strong> function returns the height of the BST, where the height of a tree is the length of the longest simple path from the root to a leaf and the root is counted as level 0.</li>

 <li>Height of tree (root level = 1). The <strong>numLevels()</strong> function returns the height of the BST, where the height of a tree is the number of levels in the tree and the root is counted as level 1.</li>

 <li> Find the node with minimum key (iteration). The <strong>findMin()</strong> function iteratively searches on the BST for the node with the smallest value <strong>m</strong> of the data member. The <strong>findMin()</strong> function returns the node containing <strong>m</strong>.</li>

 <li> Find the node with minimum key (recursion). The <strong>findMinR()</strong> function recursively searches on the BST for the node with the smallest value <strong>m</strong> of the data member. The <strong>findMinR()</strong> function returns the node containing <strong>m</strong>.</li>

 <li>Find the node with maximum key (iteration). The <strong>findMax()</strong> function iteratively searches on the BST for the node with the largest value <strong>M</strong> of the data member. The <strong>findMax()</strong> function returns the node containing <strong>M</strong>.</li>

 <li> Find the node with maximum key (recursion). The <strong>findMaxR()</strong> function recursively searches on the BST for the node with the largest value <strong>M</strong> of the data member. The <strong>findMaxR()</strong> function returns the node containing <strong>M</strong>.</li>

 <li>Delete a node from BST (iteration). The <strong>Delete()</strong> function iteratively deletes an arbitrary node of the BST. Specifically, the program asks the user to enter the data member <strong>x</strong> of the node to be deleted. The <strong>Delete()</strong> function performs the deletion operation if <strong>x</strong> exists in the tree and returns 1; otherwise 0 is returned. The to-be-deleted node <strong>x</strong> is replaced with the leftmost node of the right subtree of <strong>x</strong>.</li>

 <li>Delete a node from BST (recursion). The <strong>DeleteR()</strong> function recursively deletes an arbitrary node of the BST. Specifically, the program asks the user to enter the data member <strong>x</strong> of the node to be deleted. The <strong>DeleteRR()</strong> function performs the deletion operation if <strong>x</strong> exists in the tree and returns the new tree (i.e., the tree with <strong>x</strong> has been deleted); otherwise displays the message “Not found”. The to-be-deleted node <strong>x</strong> is replaced with the leftmost node of the right subtree of <strong>x</strong>.</li>

 <li> Find     the       inorder             successor         (without          using    parent link).    The <strong>inOrderSuccessor()</strong> function allows the user to find the inorder successor of a given node in the BST. The inorder successor of a given node is the node comes after the node in the inorder traversal of the BST. The rightmost node of the BST has no inorder successor.</li>

 <li>Breadth-first traversal (BFT). The <strong>BFT()</strong> function traverses the tree level by level, staring at the root. At each level, the nodes are traversed from left to right.</li>

 <li>Quit your program.</li>

 <li><strong> Part 2</strong> Hashing methods</li>

</ol>

Write the following complete C (or C++) programs.

<ol>

 <li><strong>c</strong> to implement the linear probing method.</li>

 <li><strong>c</strong> to implement the quadratic probing method.</li>

 <li><strong>c</strong> to implement the double hashing method.</li>

 <li><strong>c</strong> to implement the coalesced chaining method.                                <strong>5</strong>. <strong>SC.c</strong> to implement the separate/direct chaining method.</li>

</ol>

<ul>

 <li>Each of the above programs should displays the following menu when it is executed.</li>

</ul>

<ol>

 <li>Insert a new key</li>

 <li>Search a given key</li>

 <li>Delete a given key</li>

 <li>Display hash table</li>

 <li>Quit</li>

</ol>

Select your option (1-5):




<ul>

 <li>Each of the above programs has the <strong>Insert()</strong>, <strong>Search()</strong>, <strong>Delete()</strong>, and <strong>Display()</strong> functions to perform the insertion, searching, deletion, and displaying operations, respectively. The <strong>Insert()</strong> function allows a user to insert a new key <strong>k</strong> into the hash table. It is supposed that the keys are distinct nonnegative integers. The <strong>Search()</strong> function allows a user to search the hash table for a given key <strong>k</strong>. The <strong>Delete()</strong> function allows a user to delete a given key <strong>k</strong> from the hash table. The <strong>Display()</strong> function shows the hash table contents on the screen.</li>

</ul>




<ul>

 <li>For the <strong>c</strong> program, the size of the hash table is <em>M</em> = 10. The hash function is defined as <em>f</em>(<em>k</em>)</li>

</ul>

= <em>k</em> % <em>M</em>, where the symbol % is the modulo operator and the key <em>k</em> is a nonnegative integer. The rehash function is <em>f<sub>t</sub></em>(<em>k</em>) = (<em>f</em>(<em>k</em>) + <em>t</em>) % <em>M</em>, where the collision count <em>t</em> = 1, 2, …. The <strong>Search()</strong> function returns the index <em>i</em> of <strong>k</strong>, 0 ≤ <em>i</em> ≤ <em>M</em> – 1, if <strong>k</strong> is found; otherwise, returns <em>M</em>. Each node of the hash table is defined by <strong>typedef struct { int k; } Node;</strong>.




<ul>

 <li>For the <strong>c</strong> program, the size of the hash table is <em>M</em> = 10. The hash function is defined as <em>f</em>(<em>k</em>)</li>

</ul>

= <em>k</em> % <em>M</em>, where the symbol % is the modulo operator and the key <em>k</em> is a nonnegative integer. The rehash function is <em>f<sub>t</sub></em>(<em>k</em>) = (<em>f</em>(<em>k</em>) + <em>t</em><sup>2</sup>) % <em>M</em>, where the collision count <em>t</em> = 1, 2, …. The <strong>Search()</strong> function returns the index <em>i</em> of <strong>k</strong>, 0 ≤ <em>i</em> ≤ <em>M</em> – 1, if <strong>k</strong> is found; otherwise, returns <em>M</em>. Each node of the hash table is defined by <strong>typedef struct { int k; } Node;</strong>.




<ul>

 <li>For the <strong>c</strong> program, the size of the hash table is <em>M</em> = 11. The hash function is defined as <em>f</em>(<em>k</em>) = <em>k</em> % <em>M</em>, where the symbol % is the modulo operator and the key <em>k</em> is a nonnegative integer. The rehash function is <em>f<sub>t</sub></em>(<em>k</em>) = (<em>f<sub>t</sub></em><sub>-1</sub>(<em>k</em>) + <em>g</em>(<em>k</em>)) % <em>M</em>, where the collision count<em> t</em> = 1, 2, …., the second hash function is <em>g</em>(<em>k</em>) = <em>c</em> – (<em>k</em> % <em>c</em>), the constant <em>c</em> = 5, <em>f</em><sub>0</sub>(<em>k</em>) = <em>f</em>(<em>k</em>). The <strong>Search()</strong> function returns the index <em>i</em> of <strong>k</strong>, 0 ≤ <em>i</em> ≤ <em>M</em> – 1, if <strong>k</strong> is found; otherwise, returns <em>M</em>. Each node of the hash table is defined by <strong>typedef struct { int k; } Node;</strong>.</li>

</ul>




<ul>

 <li>For the <strong>c</strong> program, the size of the hash table is <em>M</em> = 10. The <strong>Search()</strong> function returns the index <em>i</em> of <strong>k</strong>, 0 ≤ <em>i</em> ≤ <em>M</em> – 1, if <strong>k</strong> is found; otherwise, returns <em>M</em>. The <strong>Delete()</strong> function works as the following illustration. Each node of the hash table is defined by <strong>typedef struct { int k; int next; } Node;</strong>.</li>

</ul>

Suppose that the current state of the hash table is as follows.




<table width="0">

 <tbody>

  <tr>

   <td width="59">Index</td>

   <td width="38"><em>k </em></td>

   <td width="49"><em>next </em></td>

   <td rowspan="11" width="66"> </td>

   <td width="59">Index</td>

   <td width="38"><em>k </em></td>

   <td width="49"><em>next </em></td>

   <td rowspan="11" width="66"> </td>

   <td width="59">Index</td>

   <td width="38"><em>k </em></td>

   <td width="49"><em>next </em></td>

  </tr>

  <tr>

   <td width="59">0</td>

   <td width="38">10</td>

   <td width="49">9</td>

   <td width="59">0</td>

   <td width="38">10</td>

   <td width="49"><strong>-1</strong></td>

   <td width="59">0</td>

   <td width="38"><strong>30 </strong></td>

   <td width="49"><strong>-1</strong></td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">1</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">1</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">2</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">2</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">2</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">3</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">3</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">3</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">4</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">4</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">4</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">5</td>

   <td width="38">15</td>

   <td width="49">8</td>

   <td width="59">5</td>

   <td width="38">15</td>

   <td width="49">8</td>

   <td width="59">5</td>

   <td width="38">15</td>

   <td width="49">8</td>

  </tr>

  <tr>

   <td width="59">6</td>

   <td width="38">26</td>

   <td width="49">-1</td>

   <td width="59">6</td>

   <td width="38">26</td>

   <td width="49">-1</td>

   <td width="59">6</td>

   <td width="38">26</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">7</td>

   <td width="38">35</td>

   <td width="49">-1</td>

   <td width="59">7</td>

   <td width="38">35</td>

   <td width="49">-1</td>

   <td width="59">7</td>

   <td width="38">35</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">8</td>

   <td width="38">25</td>

   <td width="49">7</td>

   <td width="59">8</td>

   <td width="38">25</td>

   <td width="49">7</td>

   <td width="59">8</td>

   <td width="38">25</td>

   <td width="49">7</td>

  </tr>

  <tr>

   <td width="59">9</td>

   <td width="38">30</td>

   <td width="49">-1</td>

   <td width="59">9</td>

   <td width="38"><strong>-1 </strong></td>

   <td width="49">-1</td>

   <td width="59">9</td>

   <td width="38"><strong>-1 </strong></td>

   <td width="49">-1</td>

  </tr>

 </tbody>

</table>

Initial state                                If 30 is deleted.                            If 10 is deleted.
















<table width="0">

 <tbody>

  <tr>

   <td width="59">Index</td>

   <td width="38"><em>k </em></td>

   <td width="49"><em>next </em></td>

   <td rowspan="11" width="66"> </td>

   <td width="59">Index</td>

   <td width="38"><em>k </em></td>

   <td width="49"><em>next </em></td>

   <td rowspan="11" width="66"> </td>

   <td width="59">Index</td>

   <td width="38"><em>k </em></td>

   <td width="49"><em>next </em></td>

  </tr>

  <tr>

   <td width="59">0</td>

   <td width="38">10</td>

   <td width="49">9</td>

   <td width="59">0</td>

   <td width="38">10</td>

   <td width="49">9</td>

   <td width="59">0</td>

   <td width="38">10</td>

   <td width="49">9</td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">1</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">1</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">2</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">2</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">2</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">3</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">3</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">3</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">4</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">4</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

   <td width="59">4</td>

   <td width="38">-1</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">5</td>

   <td width="38">15</td>

   <td width="49">8</td>

   <td width="59">5</td>

   <td width="38">15</td>

   <td width="49">8</td>

   <td width="59">5</td>

   <td width="38"><strong>25 </strong></td>

   <td width="49">8</td>

  </tr>

  <tr>

   <td width="59">6</td>

   <td width="38">26</td>

   <td width="49">-1</td>

   <td width="59">6</td>

   <td width="38">26</td>

   <td width="49">-1</td>

   <td width="59">6</td>

   <td width="38">26</td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">7</td>

   <td width="38"><strong>-1 </strong></td>

   <td width="49">-1</td>

   <td width="59">7</td>

   <td width="38"><strong>-1 </strong></td>

   <td width="49">-1</td>

   <td width="59">7</td>

   <td width="38"><strong>-1 </strong></td>

   <td width="49">-1</td>

  </tr>

  <tr>

   <td width="59">8</td>

   <td width="38">25</td>

   <td width="49"><strong>-1 </strong></td>

   <td width="59">8</td>

   <td width="38"><strong>35 </strong></td>

   <td width="49"><strong>-1 </strong></td>

   <td width="59">8</td>

   <td width="38"><strong>35 </strong></td>

   <td width="49"><strong>-1 </strong></td>

  </tr>

  <tr>

   <td width="59">9</td>

   <td width="38">30</td>

   <td width="49">-1</td>

   <td width="59">9</td>

   <td width="38">30</td>

   <td width="49">-1</td>

   <td width="59">9</td>

   <td width="38">30</td>

   <td width="49">-1</td>

  </tr>

 </tbody>

</table>

If 35 is deleted.                            If 25 is deleted.                            If 15 is deleted.




<ul>

 <li>For the <strong>c</strong> program, the size of the hash table is <em>M</em> = 10. The <strong>Search()</strong> function returns the pointer to the node containing <strong>k</strong> if <strong>k</strong> is found; otherwise, returns <strong>NULL</strong>. Each node of the</li>

</ul>

hash table is defined by <strong>typedef struct { int k; struct Node *next; } Node;</strong>.