Download Link: https://assignmentchef.com/product/solved-cs-2413-data-structures-programming-project-2
<br>
<h1></h1>

The goal of this project is to create extend the DataFrame class in C++ developed in Project 1 as outlined in the project description. Document your project thoroughly as the examples in the textbook (20 point penalty for poor documentation). This includes but not limited to brief header comments for all classes/methods, explanatory comments for each section of code, meaningful variable and method names, and consistent indentation. Project Description

In this project you will create a new templated DataFrame class along with the all the methods that are represented in the class definition.  DataFrame is a table with rows and columns – columns have names associated with them.  Each row of the DataFrame is a single &lt;DT&gt; (RowObject in this case), so the DataFrame maintains an array of pointers to RowObject.  The RowObject class is also defined below.

After you have tested your class, you have to execute the main program that is also given below.

<h2>RowObject Class</h2>

<h2>DataFrame Class</h2>

template &lt;class DT&gt; class DataFrame { protected:

DT** dataRows; // array of pointers to DT object

char** colNames; int noRows, noCols; public:

DataFrame ();

DataFrame(int numberOfRows, int numberOfColumns); void display();

void display(int n); // display the first n records void setColName(int col, const char* name); DT&amp; operator[] (int i); //get the ith row char** getColNames(); int getNumberRows();

DataFrame&lt;DT&gt;* getRows(int* rows, int rLen);

void addRow(DT&amp; newRow); // add a new row at the last row

void removeRow(int i); //remove the ith row void insertRow(int position, DT&amp; newRow);

void ~DataFrame();

//write the ostream operator

//write the = operator for an extra 10 points

};

<h2>The main function</h2>

// Write all the methods here and execute the following main program with some code that you need to write.

<h1>Constraints</h1>

<ol>

 <li>In this project, the only header you will use is #include &lt;iostream&gt;.</li>

 <li>None of the projects is a group project. Consulting with other members of this class on programming projects is strictly not allowed and plagiarism charges will be imposed on students who do not follow this.</li>

</ol>