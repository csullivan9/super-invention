# X-Team 18 Style Guide

<brief description of your team's opinion or philosophy regarding Style Guides>

## Naming conventions

* Be consistent.
* Names should use camelCase.
* Method names that are over 3 words in length should use underscores.
* Names should of course be relevant to their function.
* Classes, interfaces, exception types should start with a capital letter.

### Examples
* interfaces
    * public interface SearchTreeADT {}
* classes
    * public class BalancedSearchTree {}
* exception types
    * EmptyQueueException
* fields
    * private int heightOfTree;
* methods
    * public void test01_isEmpty_on_empty_tree() {}
    * public String toString() {}
* parameters
    * (Treenode<T> rootOfSubtree)
* local variables
    * int leftNodeIndex;
* instance constants
    * private final double exponentIncrement;
* class constants
    * private static final double piValue = 3.14;


## Commenting style for public and private members of a class or interface:

* Be consistent.
* In-line comments should have descriptions for complex blocks of code and algorithms.
* Comments for public members of classes.
* Comments should add information to otherwise obscure blocks of code.
* Javadoc for methods is not required and optional.

### Examples

* classes
    * // inner node class to store key items and links to other nodes
    * protected class Treenode<K extends Comparable<K>> {}
* fields
    * // pointer node to parent node of current state
    * private State pointer;
* constructors
    * // constructs a Treenode with item as key and null for left and right children
    * public Treenode(K item) {
        * this(item, null, null);
    * }
* methods
    * // rotates subtree of node left using algorithm from class
    * private Treenode<T> leftRot(Treenode<T> node) {}


* coding style (brackets, horizontal, and vertical spacing) for:
  * if statements
      * if(( bool && (3 >= 5)) || !boolValue) {
          * intValue = 5;
      * } else {
          * return;
      * }
  * switch statement
      * switch (month) {
          * case 1:  monthString = "January";
              * break;
          * case 2:  monthString = "February";
              * break;
          * default: monthString = "Invalid month";
              * break;
      * }
  * while loops
      * while(true) {
          * intValue++;
      * }
  * for loops
      * for(int i = 0; i < str.length; i++) {
          * array.add(i);
      * }
  * enhanced for loops
      * for(State successor : successors) {
          * stack.push(successor);
      * }
  
