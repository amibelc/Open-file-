# Open-file-
open file and add text. 

//handling file 
#include <iostream>
#include <fstream>
using namespace std;

int main()
{
    fstream myFile;
    myFile.open("amina.txt", ios::out); //write
    if(myFile.is_open()){
        myFile <<"Hello\n";
        myFile <<"This is second line\n";
        myFile.close();
    }
     myFile.open("amina.txt", ios::app); //append
    if(myFile.is_open()){
        myFile <<"Hello2\n";
        myFile <<"This is second line\n";
        myFile.close();
    }

    system("pause>0");
}
