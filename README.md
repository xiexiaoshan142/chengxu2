# chengxu2
#include<iostream>
#include<fstream>
using namespace std;
int mian()
{
   int sum=0,progone[100],i=0;
   ifstream open("D:/shuju.txt");
   if(!open)
   {
        cout<<"不能打开文件！/n";
    }
    while(open>>progone[i],i<100)
    {
         sum+=progone[i];
         i++;
     }
     cout<<"数组中100个元素的和为:"<<sum<<endl;
     open.close();
     return 0;
}
