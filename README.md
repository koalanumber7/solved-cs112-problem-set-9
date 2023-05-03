Download Link: https://assignmentchef.com/product/solved-cs112-problem-set-9
<br>
<strong>Problem Set 9</strong>

<strong>Hash Table</strong>

<ol>

 <li>You are given the following keys to be hashed into a hash table of size 11:</li>

</ol>

96,  43,  72,  68,  63,  28 Assume the following hash function is used      H(key) = key mod 11

and chaining (array of linked lists) is used to resolve collisions.

<ol>

 <li>Show the hash table that results after all the keys are inserted.</li>

 <li>Compute the average number of comparisons for successful search.</li>

</ol>

<ol start="2">

 <li>Using chaining to resolve collisions, give the worst-case running time (big O) for inserting <em>n</em> keys into an initially empty hash table table for each of the following kinds of chains:</li>

 <li>Using the following class definitions:</li>

</ol>

class Node {           int key;           String value;

Node next;

}

class Hashtable {           Node[] entries;           int numvalues;           float max_load_factor;

public Hashtable(float max_load_factor) { … } // constructor       }

Complete the following methods of the Hashtable class, using the hash function h(key) = key <strong>mod</strong> table_size.

public void insert(int key, String value) {

// COMPLETE THIS METHOD

}

private void rehash() {          // COMPLETE THIS METHOD       }

Note: When expanding the hash table, double its size.

<ol start="4">

 <li><strong>*</strong> Suppose you are asked to write a program to count the frequency of occurrence of each word in a document. Desrcibe how you would implement your program using:</li>

 <li>A hash table to store words and their frequencies.</li>

 <li>An AVL tree to store words and their frequencies.</li>

</ol>

For each of these implementations:

<ol>

 <li>What would be the worst case time to populate the data structure with all the words and their frequencies?</li>

 <li>What would be the worst case time to look up the frequency of a word?</li>

 <li>What would be the worst case time to print all words and their frequencies, in alphabetical order of the words?</li>

</ol>

Assume there are <em>n</em> distinct words in the document, and a total of <em>m</em> words, and <em>m</em> is much greater than <em>n</em>.