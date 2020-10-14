# The programs
I've loaded 2 programs: MyPercep is the learning algorithm that saves on a file the weight vector, while Output Produced reads the weight vector (from the previous file) and an input from the user producing a scalar output between -1 (false) and 1 (true).

This is only an example but it can be useful to understand some easy applications and (most importantly) the limits of Perceptron (es the XOR problem)
# The functions (fast guide for the user):
CONTROLEX(float*) : takes a pointer 1D in input and prints an error message if the pointer is NULL (useful after allocation);

NEXANDIN(int*,int*) : takes in input 2 pointers: 1° is the row of the input matrix and is the number of examples you want to use, 2° is the column of the input matrix and is the number of elements that are in each example (or equivalently the number of connections of the "firing neuron");

INPUT(float**,int*,int*) : fills the input matrix with the data stored in a selected file;

INPUTEPS(float*,int*) : loads the correct answers of the problem from a file;

SCALPROD(float**,float*,int*,int) : does the scalar product from the (ind)th row vector of the matrix and the weight vector;

ERRORF(float*,float*,int*) : calculates the error between the correct answers and the produced answers (quadratic cost function);

HEBB (float**,float*,float*,float*,int*,int) : applies the Hebb's rule to the weight vector for the learning process;

PERCEPTRON(float**,float*,int*,int*) : uses the input matrix and the vector with correct answers to produce and save a weight vector that satisfy the requirements imposed (if exist a solution!).  
# Recommended book
Introduction to the theory of neural computation - Krogh Anders, Hertz John, Palmer Richard
