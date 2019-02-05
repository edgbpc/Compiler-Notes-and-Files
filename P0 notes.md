#  P0 Notes

PROJECT 0 -

ctrl+d to simulate end of file

Standard template library. (Stl)

c++ strings


Abstract syntax tree

Adam ala ada Jim ala Susan George Georg john



0   4: Adam
         john
1        3: Ala        5: Susan
              Ada           Georg
              Jim
2                         6: George


Print preorder traversal - visit node, process node before traveling left, then down (if nothing left or right returns up a node and checks right)
4 Adam John                4 - root
3 Ala Ada Jim                3 - child of root, has no children
5 Susan Georg                5 - child of root, has a child 6
6 George


MUST USE FUNCTION NAMES IN ASSIGNMENTS

Write program to only read from file

If keyboard input, take input from keyboard and save to file then read file

If redirection -  //name of program is 1st argument argc =1
Int main(int argc, char * argv[]){

//process # of argument
If argc > 2  //error too many arguments

If argc == 2  {//file basename given
string base = argv[1]
base += ".sp19"

FILE *fp = fopen(base, "r")
//test if not successfully open
}

If argc == 1 {//keyboard or the redirection
fp = stdin

}
String data
Fscanf(fp, "%s", data)  //fp is file pointer either from the file or the keyboard, but doesn't matter

}

Simulate end of file usually  -1/EOF -p not physically in the file but how the utility reads it
person at keyboard has to enter a simulated end of file - usually ctrl - d on linux(delmar)
redirection tells shell to substitutie for keyboard


stcat(argv[1], ".sp19") //won't work in C but in C++ should extend size of argv[1] to accomodate

fopen(argv[1])





