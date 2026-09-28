
#include<bits/stdc++.h>
using namespace std;

class Delivery
{
public:
    void charge(double w)
        {cout<<"Local Charge: "<<w*90<<endl;
        }
    void charge(double w,double d)
    {
        cout<<"Long Charge: "<<w*d*10<<endl;
    }

    void charge(double w,double d,double c)
    {
        cout<<"International Charge: "<<(w*d*10)+c<<endl;
    }
};

int main()
{
    Delivery ob1;
    ob1.charge(5);
    ob1.charge(5,100);
    ob1.charge(5,100,500);

    return 0;
}
