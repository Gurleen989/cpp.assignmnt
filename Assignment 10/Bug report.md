I  did not get any error while running the code but  below I will mention some possible bugs that could have resulted into error .

# Bug 1

1. **The incorrect original code or code snippit that you wrote:**

``` cpp
//code with bugs or code snippet with bug goes here

//sample code

// Online C++ compiler to run C++ online.
// Write C++ code in this online editor and run it

#include <iostream>
#include <fstream>
using namespace std;
int main
{
    string FileName;
    string h;
    int n, i=0;
    cout<<"Enter the FileName:";
    cin>>FileName;
    cout<<"Enter the Integer Number:";
    cin>>n;
    // opening the file in read mode
    ifstream in(FileName.c_str());
    if(! in.good())
    {
        cout<<"ERROR :Invalid FileName";
        exit(0);
    }
    while((!in.eof())&&(i<n))
    {
        //in order to read file
        getline(in,h);
        cout<<h<<endl ;
        i++;
    }

    if(i<n)
    cout<<"Entire file is displayed"<<endl ;

}

```

2. **What bug does the original code have?**

  Ans . One can get error in the fourth line for not putting braces after main which will result into error like cannot declare main to be a global variable which will ask for primary expression before file name .

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

   Ans . One can make this mistake due to lack of knowledge or in hurriness . I used to make this when I started coding which used to take my most of the time .

4. **How to correct the bug?**

   Ans . By using simple braces () in 4th line after main , the bug can be corrected .

5. **The corresponding bug-free code or code snippet is:**

```
bug-free code or code snippet goes here
#include <iostream>
#include <fstream>
using namespace std;
int main()
{
    string FileName;
    string h;
    int n, i=0;
    cout<<"Enter the FileName:";
    cin>>FileName;
    cout<<"Enter the Integer Number:";
    cin>>n;
    // opening the file in read mode
    ifstream in(FileName.c_str());
    if(! in.good())
    {
        cout<<"ERROR :Invalid FileName";
        exit(0);
    }
    while((!in.eof())&&(i<n))
    {
        //in order to read file
        getline(in,h);
        cout<<h<<endl ;
        i++;
    }

    if(i<n)
    cout<<"Entire file is displayed"<<endl ;

}


```

6. **What is the take-away message from this bug?**

   Ans . Users write this function ( main()) in program to start the execution. Apart from that , Brackets () are used because it is the parenthesis which is used for a function . By this , one can pass on the values from one function to another function by mentioning name and type of variable in the parenthesis . 

---

I  did not get any error while running the code but  below I will mention some possible bugs that could have resulted into error .

# Bug 2

1. **The incorrect original code or code snippit that you wrote:**

```
code with bugs or code snippet with bug goes here
#include <iostream>
#include <fstream>
using namespace std;
int main()
{

    int n, i=0;
    cout<<"Enter the FileName:";
    cin>>FileName;
    cout<<"Enter the Integer Number:";
    cin>>n;
    // opening the file in read mode
    ifstream in(FileName.c_str());
    if(! in.good())
    {
        cout<<"ERROR :Invalid FileName";
        exit(0);
    }
    while((!in.eof())&&(i<n))
    {
        //in order to read file
        getline(in,h);
        cout<<h<<endl ;
        i++;
    }

    if(i<n)
    cout<<"Entire file is displayed"<<endl ;

}


```

2. **What bug does the original code have?**

  Ans. One can get the error by not declaring the variables after int main () which can further lead to the words written in further statements to give the error like FileName  is not declared  in this scope.

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

   Ans .One can have any misunderstanding about that or lack of knowledge .

4. **How to correct the bug?**

   Ans .  By declaring the variables after int main (), one can correct the bug.

5. **The corresponding bug-free code or code snippet is:**

```
bug-free code or code snippet goes here
#include <iostream>
#include <fstream>
using namespace std;
int main()
{
    string FileName;
    string h;
    int n, i=0;
    cout<<"Enter the FileName:";
    cin>>FileName;
    cout<<"Enter the Integer Number:";
    cin>>n;
    // opening the file in read mode
    ifstream in(FileName.c_str());
    if(! in.good())
    {
        cout<<"ERROR :Invalid FileName";
        exit(0);
    }
    while((!in.eof())&&(i<n))
    {
        //in order to read file
        getline(in,h);
        cout<<h<<endl ;
        i++;
    }

    if(i<n)
    cout<<"Entire file is displayed"<<endl ;

}

```

6. **What is the take-away message from this bug?**

   Ans. .It is mandatory to declare variables after int main () so that they are always initialised to any value which is valid .

   Apart from that ,One should do practice and one should do the compiling with full concentration , so that , they will not make such type of mistakes in hurry . Apart from that , if one gets any error ,he /she should get proper information about why they are getting this error and should try not to repeat that mistake again .

---

I  did not get any error while running the code but  below I will mention some possible bugs that could have resulted into error .

# Bug 3

1. **The incorrect original code or code snippit that you wrote:**

```
code with bugs or code snippet with bug goes here
#include <iostream>
#include <fstream>
using namespace std;
int main()
{
    string FileName;
    string h;
    int n, i=0;
    cout<<"Enter the FileName:"
    cin>>FileName;
    cout<<"Enter the Integer Number:";
    cin>>n;
    // opening the file in read mode
    ifstream in(FileName.c_str());
    if(! in.good())
    {
        cout<<"ERROR :Invalid FileName";
        exit(0);
    }
    while((!in.eof())&&(i<n))
    {
        //in order to read file
        getline(in,h);
        cout<<h<<endl ;
        i++;
    }

    if(i<n)
    cout<<"Entire file is displayed"<<endl ;

}

```

2. **What bug does the original code have?**

  Ans . One can get error if one does not terminate the derived class like in 9th line , one can get error for not putting semicolon.

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

   Ans . They can  forget to put that at end  while compiling the program or lack of knowledge can be responsible .

4. **How to correct the bug?**

   Ans . By putting the semicolon in the 9th line, the bug can be corrected .

5. **The corresponding bug-free code or code snippet is:**

```
bug-free code or code snippet goes here
#include <iostream>
#include <fstream>
using namespace std;
int main()
{
    string FileName;
    string h;
    int n, i=0;
    cout<<"Enter the FileName:";
    cin>>FileName;
    cout<<"Enter the Integer Number:";
    cin>>n;
    // opening the file in read mode
    ifstream in(FileName.c_str());
    if(! in.good())
    {
        cout<<"ERROR :Invalid FileName";
        exit(0);
    }
    while((!in.eof())&&(i<n))
    {
        //in order to read file
        getline(in,h);
        cout<<h<<endl ;
        i++;
    }

    if(i<n)
    cout<<"Entire file is displayed"<<endl ;

}

```

6. **What is the take-away message from this bug?**

Ans. Semi-colon is used at end of curly braces of class in C++ because the compiler needs the ; to know you do not want to  declare variables after the class declaration .