# ALL-PF-LAB-TASKS 
TASK 1:
#include<stdio.h>
int main ()
{
    int att;
    printf("Please enter your attendance percentage:");
    scanf("%d",&att);
    if(att>75)
    {
        printf("Eligible for exams! ");
    }
    else
    {
        printf("Ineligible! ");

}
return 0;
}

TASK # 2:
#include<stdio.h>
int main()
{
    int units;
    printf ("Please enter the units:");
    scanf("%d",&units);
    if(units<=100)
    {
        printf("Low Usage!");
    }
    else if(units<=300)
    {
        printf("Medium Usage!");
    }
    else 
    {
        printf("High Usage!");
    }
}

TASK # 3

#include<stdio.h>
int main()
{
    int number;
    printf ("Please enter the number:");
    scanf("%d",&number);
    if(number>0)
    {
        printf("Positive!");
    }
    else if(number<0)
    {
        printf("Negative");
    }
    else 
    {
        printf("Zero");
}
return 0;
}

TASK # 4:
#include <stdio.h>

int main()
{
    int U_pwd;
    char U_name[20];

    printf("Please enter your User name:\n");
    scanf("%s", U_name);

    printf("Please enter your Password:\n");
    scanf("%d", &U_pwd);

    if (
    U_name[0]=='a' &&
    U_name[1]=='d' &&
    U_name[2]=='m' &&
    U_name[3]=='i' &&
    U_name[4]=='n' &&
    U_name[5]=='\0'&&
    U_pwd == 1234)
    {
        printf("Login successful!\n");
    }
    else
    {
        printf("Invalid credentials\n");
    }

    return 0;
}

TASK 5:
#include <stdio.h>
int main() {
    int choice;
    float amount, withdrawed, deposited;
    amount= 2890;

    printf("Press 1 for Balance Inquiry\n");
    printf("Press 2 for Cash Withdrawal\n");
    printf("Press 3 for Deposit\n");
    printf("Press 4 for Exit\n");
scanf("%d", &choice);

    switch(choice)
    {
        case 1:
        {
            printf("Your current bank balance is: %f\n",amount);
            break;
        }
        case 2:
        {
            printf("Enter the amount you want to withdraw\n");
            scanf("%f",&withdrawed);

            if(withdrawed<=amount)
            {
                amount=amount-withdrawed;
                printf("Amount withdrawn successfully, Remaining balance: %f\n",amount);
            }
            else
            {
                printf("Insufficient balance\n");
            }
            break;
        }

        case 3:
        {
            printf("Enter the amount to be deposited: ");
            scanf("%f", &deposited);
            amount= amount+deposited;
            printf("Deposit successful, New balance: %f\n",amount);
            break;
        }

        case 4:
        {
            printf("You are now exiting the program.....\n");
            break;
        }

        default:
        {
            printf("Invalid Choice\n");
        }
    }
    return 0;

TASK # 6:
#include<stdio.h>
int main()
{
    int sub1;
    int sub2;
    int sub3;
    int sub4;
    int sub5;
    
    int Tsum;
    printf ("Please enter your marks:");
    scanf("%d",&sub1);
    printf ("Please enter your marks:");
    scanf("%d",&sub2);
    printf ("Please enter your marks:");
    scanf("%d",&sub3);
    printf ("Please enter your marks:");
    scanf("%d",&sub4);
    printf ("Please enter your marks:");
    scanf("%d",&sub5);
    
    Tsum=((sub1+sub2+sub3+sub4+sub5)/5);
    if(Tsum>=85)
    {
        printf("Grade = A");
    }
    else if(Tsum>=70)
    {
        printf("Grade = B");
    }
    else if(Tsum>=50) 
    {
        printf("Grade = C");  
    }
    else
    {
        printf("You failed!");
    }
    return 0;

TASK # 7
#include <stdio.h>
int main() {
    float amount;

    printf("Please enter your itmes total purchase amount ");
    scanf("%f", &amount);
    if( amount>=5000)
    {
        amount=amount*0.8;
        printf("Your items discounted price is now %d\n ",amount);
    }
    else if (amount>=3000)
    {
        amount=amount*0.9;
        printf("Your items discounted price is now %d\n ",amount);
    }
    else
    {
        printf("Your items price is %d\n ",amount);
    }
    return 0;
}

TASK # 8
#include <stdio.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int choice;
    int a,b;
    int add,sub,product;
    double div,sq,cube,square_root,power;
    int absolute;
    
    printf("Press 1 for Addition\n");
    printf("Press 2 for Subtraction\n");
    printf("Press 3 for Multiplication\n");
    printf("Press 4 for Division\n");
    printf("Press 5 for Square of a number\n");
    printf("Press 6 for cube of a number\n");
    printf("Press 7 for Square root of a number\n");
    printf("Press 8 for Power (xy)\n");
printf("Press 9 for Absolute Value\n");

scanf("%d", &choice);

    switch(choice)
    {
        case 1:
        {
            printf("Please input two numbers:\n");
            scanf("%d%d",&a,&b);
            add=a+b;
            printf("The addition of the two numbers %d and %d is %d",a,b,add);
            break;
        }

        case 2:
        {
            printf("Please input two numbers:\n");
            scanf("%d%d",&a,&b);
            sub=a-b;
            printf("The difference between the two numbers %d and %d is %d",a,b,sub);
            break;
        }

        case 3:
        {
            printf("Please input two numbers:\n");
            scanf("%d%d",&a,&b);
            product=a*b;
            printf("The product of the two numbers %d and %d is %d",a,b,product);
            break;
        }



        case 4:
        {
            printf("Please input two numbers:\n");
            scanf("%d%d",&a,&b);
            if(b==0)
            {
                printf("Division by zero is not possible!\n");
            }
            else
            {
                div=(double)a/b;
                printf("The division of the two numbers %d and %d is %.2lf",a,b,div);
            }
            break;
        }

        case 5:
        {
            printf("Please input a number:\n");
            scanf("%d",&a);
            sq=a*a;
            printf("The square of the number %d is %.2lf",a,sq);
            break;
        }

        case 6:
        {
            printf("Please input a number:\n");
            scanf("%d",&a);
            cube=a*a*a;
            printf("The cube of the number %d is %.2lf",a,cube);
            break;
        }

        case 7:
        {
            printf("Please input a number:\n");
            scanf("%d",&a);
            if(a<0)
            {
                printf("Square root of a negative number is not possible!\n");
            }
            else
            {
                square_root=sqrt(a);
                printf("The square root of the number %d is %.2lf",a,square_root);
            }
            break;
        }

        case 8:
        {
            printf("Please input two numbers:\n");
            scanf("%d%d",&a,&b);
            power=pow(a,b);
            printf("The power of %d raised to %d is %.2lf",a,b,power);
            break;
        }

        case 9:
        {
            printf("Please input a number:\n");
            scanf("%d",&a);
            absolute=abs(a);
            printf("The absolute value of the number %d is %d",a,absolute);
            break;
        }

        default:
        {
            printf("Invalid choice!");
        }
}

    return 0;
}
    

