#include<bits/stdc++.h>

using namespace std;
//Implement the class Box  
//l,b,h are integers representing the dimensions of the box

// The class should have the following functions : 

// Constructors: 
// Box();
// Box(int,int,int);
// Box(Box);

class Box{
    private:
        long length =0; 
        long breadth = 0; 
        long height = 0;
        
        long long volume;
    public:
        Box(){}
        Box(int l, int b, int h):length(l),breadth(b),height(h){}
        Box(const Box &b){
            length = b.length;
            breadth = b.breadth;
            height = b.height;
        }
        int getLength(void){
            return length;
        }
        int getBreadth(void){
            return breadth;
        }
        int getHeight(void){
            return height;
        }
        long long CalculateVolume(void){
            volume = length*height*breadth;
            return volume;
        }
        friend std::ostream& operator<<(std::ostream& out, const Box& b){
            return out << b.length << " " << b.breadth << " " << b.height;
        }
        friend bool operator<(Box& a, Box& b){
            if((a.length < b.length) || 
            ((a.breadth < b.breadth) && (a.length < b.length))||
            (a.height < b.height && a.breadth < b.breadth && a.length == b.length))
              { return true;}
            else {return false;}
        }
};


// int getLength(); // Return box's length
// int getBreadth (); // Return box's breadth
// int getHeight ();  //Return box's height
// long long CalculateVolume(); // Return the volume of the box

//Overload operator < as specified
//bool operator<(Box& b)

//Overload operator << as specified
//ostream& operator<<(ostream& out, Box& B)

