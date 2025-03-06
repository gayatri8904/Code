#include <iostream>
using namespace std;
class worker
{
    char w_name[20];
    int n_h_work;
    int pay_rate;
    float salary;
    public:
    void getdata();
    void calculate();
    void display();
};
void worker::getdata()
{
    cout<<"Enter worker name";
    cin>>w_name;
    cout<<"Enter no of hour work";
    cin>>n_h_work;
    cout<<"Enter pay rate";
    cin>>pay_rate;
    cout<<"Enter salary";
    cin>>salary;
}
void worker::calculate()
{
    salary=n_h_work*pay_rate;
}
void worker:: display()
{
cout<<"worker name"<<w_name;
cout<<"no of hour work"<<n_h_work;
cout<<"pay rate"<<pay_rate;
cout<<"salary"<<salary;
}
int main()
{
    worker w;
    w.getdata();
    w.calculate();
    w.display();
    return 0;
}
