# Which-brackets-are-balanced

You're dealing with a string consisting of brackets. Write a program to examine whether the pairs of "{", "}", "(", ")", "[", "]" are correct or balanced. This means that each opening bracket must have a corresponding closing one (and vice versa) and they must go in the correct order.

For example, the program should print true for the string [()]{}{[()()]()} and false for ()[]}.

The classic algorithm for solving this problem relies on using a stack.

create an instance of a stack;
traverse the input string;
if the current character is a starting bracket "(" or "{" or "[" then push it to the stack;
if the current is a closing bracket ")" or "}" or "]" then remove (pop) the top element from the stack. If the popped bracket does not match the starting bracket then parentheses are not balanced;
if there are some starting brackets left in the stack after completing traversal, then the parentheses are not balanced.

Sample Input:
([][])

Sample Output:
true


Sample Input:
([](){([])})

Sample Output:
true
