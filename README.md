# Finding_Num_in_array
#include<stdio.h>
void main()
{
int n;
printf("Enter the size of array :");
scanf("%d",&n);


int arr[n];

for(int i=0;i<n;i++)
{
printf("Enter [%d] array element :  ",i);
scanf("%d",&arr[i]);
}

for(int i=0;i<n;i++)
{
printf("%d ",arr[i]);
}


int x;
printf("\nEnter element to search : ");
scanf("%d",&x);



int found =0;
for(int i=0;i<n;i++)
{

if(arr[i]==x)
{
found =1;
printf("\nNumber is found at index %d",i);
break;
}

}


if(!found)
printf("Number is not found");
}
