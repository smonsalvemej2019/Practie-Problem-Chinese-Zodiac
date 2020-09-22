# Practie-Problem-Chinese-Zodiac

//
//This program lets you input a year and it will return the chinese zodiac of that year
//The program hilights basic OOP and modular arithmetic

#include <iostream>
using namespace std;//BAD PRACTICE!!!


class ZoadiacCalc{//Our only class being used
public:
    
    
    void CalcYear(int year);//method for calculating the chinese zodiac
    
    //CalcYear can alsp be a constructor
    
private:
    
    int year =0 ;
};


void ZoadiacCalc::CalcYear(int year){//method definition
    
    {
    
 
            
        int remainder = year%12;//(YEAR) mod (NUMBER OF ZODIAC SIGNS)
        
        {
        switch(remainder){//switch statement for each different remainder
                
            case 0: //This is not Year = 0;
                
                cout<<"Year of the Monkey"<<endl;
                break;
                
            case 1:
                
                cout<<"Year of the Rooster"<<endl;
                break;
                
            case 2:
                
                cout<<"Year of the Dog!"<<endl;
                break;
                
            case 3:
                
                cout<<"Year of the Pig!"<<endl;
                break;
                
            case 4:
                
                cout<<"Year of the Rat!"<<endl;
                break;
                
            case 5:
                
                cout<<"Year of the Ox!"<<endl;
                break;
                
            case 6:
                
                cout<<"Year of the Tiger!"<<endl;
                break;
                
            case 7:
                
                cout<<"Year of the Rabbit!"<<endl;
                break;
                
            case 8:
                
                cout<<"Year of the Dragon!"<<endl;
                break;
                
            case 9:
                
                cout<<"Year of the Snake!"<<endl;
                break;
                
            case 10:
                
                cout<<"Year of the Horse!"<<endl;
                break;
                
            case 11:
                
                cout<<"Year of the Goat!"<<endl;
                break;
                
        }
            return;
        }
    }
    
    
}


int main() {
    
    
    ZoadiacCalc test1;
    test1.CalcYear(2019);//we input 2019 into the method
    
    ZoadiacCalc test2;
    test2.CalcYear(1991);
    
    ZoadiacCalc test3;
    test3.CalcYear(1);
    
    ZoadiacCalc test4;
    test4.CalcYear(2034);
    
    //you can add more tests here
    
    //the program can be repurposed to work with the western Zodiac signs
    //and it can be added by adding menus and an asking the user to input the year on the console

    //Somtimes mod arithmetic can be better than a loop
    
    return 0;
}
