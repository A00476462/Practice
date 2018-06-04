# Practice
Just for practise
#include<stdio.h>
int main()
{
     int arr[20];
     int temp,sum = 0;
     for(int i = 0;i<19;i++)
     {
         cout<<"输入第"<<i<<"个数"<<endl;
         cin>>arr[i];
     }
     //rank
     for(int i = 0;i<19;i++)
     {
         for(int j = i;j<19;j++)
         {
              if(arr[i]<arr[j])
              {
                   temp = arr[i];
                   arr[i] = arr[j];
                   arr[j] = temp;
              }
         }
     }
     //output result
     cout<<"排序后的数组:"<<endl;
     for(int i = 0;i<19;i++)
     {
         cout<<arr[i]<<"   ";
         sum++
         if(sum%5==0)
         cout<<endl;   
     }
     
     

}
