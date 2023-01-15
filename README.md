# matrixprogram 
Write a program to maintain a record of „n‟ employee detail using an array of
structures with three fields(id, name , salary) and print the details of employees
whose salary is above 5000
#include<stdio.h>
struct empsal
{
    int id;
    char name[30];
    float sal;

};
int main(){
    struct empsal a[100]; 
    int i, size;
    printf("Enter the Number of the Employ\n");
    scanf("%d",&size);
    printf("Enter the Data Of the Employ\n");
    for ( i = 0; i <size; i++)
    {
    printf("Id of the %d Employ",i);
    scanf("%d",&a[i].id);
    printf("Name of the %d Employ",i);
    scanf("%s",&a[i].name);
    printf("Sal of the %d Employ",i);
    scanf("%f",&a[i].sal);
    }
    printf("The data of the Employ\n");
    printf("Id\tName\tSalriy\n");
    for ( i = 0; i <size; i++)
    {
        printf("%d\t",a[i].id);
        printf("%s\t",a[i].name);
        printf("%f",a[i].sal);
        printf("\n");
    }
    printf("The Employ Haivng Salry 5000rs\n");
     printf("Id\tName\tSalriy\n");
      for ( i = 0; i <size; i++)
    {
        if (a[i].sal>5000)
        {
    
        printf("%d\t",a[i].id);
        printf("%s\t",a[i].name);
        printf("%f",a[i].sal);
        printf("\n");
    
        }
        
    }
    
    
    
}
