# test_backend_dott

Challange:\
There is given a rectangular bitmap of size n*m. Each pixel of the bitmap is either white or black, but at least one is white. The pixel in i-th line and j-th column is called the pixel (i,j). The distance between two pixels p1=(i1,j1) and p2=(i2,j2) is defined as d(p1,p2)=|i1-i2|+|j1-j2|.\
\
This program:\
	● reads the description of the bitmap from the standard input;\
	● for each pixel, computes the distance to the nearest white;\
	● writes the results to the standard output.\
\
Input:\
The number of test cases t (1≤t≤1000) is in the first line of input, then t test cases follow.
In the first line of each test case there is a pair of integer numbers n, m separated by a single space, 1<=n <=182, 1<=m<=182.\
In each of the following n lines of the test case exactly one zero-one word of length m, the description of one line of the bitmap, is written.\
On the j-th position in the line (i+1), 1 <= i <= n, 1 <= j <= m, is '1' if, and only if the pixel (i,j) is white.\
\
Output:\
In the i-th line for each test case, 1<=i<=n, there should be written m integers f(i,1),...,f(i,m) separated by single spaces, where f(i,j) is the distance from the pixel (i,j) to the nearest white pixel.\
\
Example:\
\
Input:\
1\
3 4\
0001\
0011\
0110\
\
Output:\
\
3 2 1 0\
2 1 0 0\
1 0 0 1\
\
Requirements:\
	- Node.js -  				$ brew install node\
	- Yarn -  					$ npm install --global yarn\
\
To set up and compile run:	$ yarn install\
To run tests run:			$ yarn test\
\
Usage:\
	> App [options]\
	> cat \<path> | App\
\
Options:\
	-f, --file \<path>	input from file\
	-h, --help			display help for command\
\
Example calls:\
	$ node App.js -f \<path>\
	$ cat <path> | node App.js\
\
\
To see the program in action run the following command from the root folder:\
	$ cat ./src/tests/testFiles/bitmap.map | node ./dist/App.js