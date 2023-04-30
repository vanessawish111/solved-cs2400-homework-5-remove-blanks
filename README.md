Download Link: https://assignmentchef.com/product/solved-cs2400-homework-5-remove-blanks
<br>
Use input/output files, strings, and command line arguments

Write a program that processes a text file by removing all blank lines (including lines that only contain white spaces), all spaces/tabs before the beginning of the line, and all spaces/tabs at the end of the line. The file must be saved under a different name with all the lines numbered and a single blank line added at the end of the file.

For example, if the input file is given as follows:

The file names must be provided at the command line (see “<strong>Parsing command line arguments</strong>”  below). To use your program, a user would type:

./a.out first.txt second.txt

Where “first.txt” is the input file name and “second.txt” is the output file name.

Your program must print usage/help message and quit if any of the following occurs:

<ul>

 <li>Wrong number of arguments at the command line.</li>

 <li>The input file fails to open</li>

 <li>The output file fails to open<strong>        </strong></li>

</ul>

<strong>Your program must include, at least, the following functions: </strong>

<ul>

 <li>A function to display a usage message to the user.</li>

 <li>A function that removes all white spaces from the beginning and end of the line. Should take a string and return a string.</li>

</ul>

<strong>Parsing command line arguments </strong>

In C++ you can input data (in the form of strings) into your program on the command line (command line arguments).  You can capture these data by adding two parameters to your main program as follows:

int main (int argc, char *argv[])

argc:  (argument count) number of arguments on the line, including the name of the program argv:  (argument vector) list of c-style strings that represent all the arguments including the name of the program.

For example, executing the command:

./a.out file1.txt file2.txt

Assigns:

argc = 3

argv[0] will be “./a.out” argv[1] will be “file1.txt” argv[2] will be “file2.txt”

To get the file name into your program you would write the following code:

string inputFileName = argv[1]; string outputFileName = argv[2]; <strong>Grading: </strong>

Programs that contain syntax errors will earn zero points.

Programs that do not include the above functions will also earn zero points.

Programs that use global variables other than constants will earn zero points.

Your grade will be determine using the following criteria:

<ul>

 <li>Correctness (25 points) o 5 usage function. o 15 points: removing the white spaces function o 5 points: displaying error messages</li>

 <li>Style &amp; Documentation (5 points)</li>

</ul>