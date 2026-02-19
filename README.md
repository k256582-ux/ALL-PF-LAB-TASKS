# ALL-PF-LAB-TASKS 

## LAB 4

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


## LAB 5

TASK 1
#include<stdio.h>
int main()
{
    float cgpa;
    int income;
    
    printf("Please enter your CGPA: ");
    scanf("%f",&cgpa);
    printf("Please enter your Family income: ");
    scanf("%d",&income);

    if(cgpa>=3.5)
    {
        if(income<50000)
        {
            printf("You are elegible for a scholarship of  100%");
        }
        
        else
        {
            printf("You are elegible for a scholarship of 50% ");
        }
    }
    else
    {
        if (cgpa>=3.0 && income<40000)
        {
            printf("You are elegible for a scholarship of  25%");
        }

        else
        {
            printf("You are not elegible for a scholarship");
        }
    }
    return 0;      
        
    }



TASK 2:

#include<stdio.h>
#include<string.h>

int main()
{
    int units;
    int bill;
    char customerType[20];
    
    printf("Please enter units: ");
    scanf("%d",&units);
    printf("Please enter the customer type: ");
    scanf("%s",customerType);

    if(units<=100)
    {
        bill=10*units;
        printf("Your bill is %d",bill);
    }
    
    else
    {
        if(units<=300)
        {
            if(strcmp(customerType,"domestic")==0)
            {
                bill=12*units;
                printf("Your bill is %d",bill);
            }
            
            else
            {
                if(strcmp(customerType,"commercial")==0)
                {
                    bill=15*units;
                    printf("Your bill is %d",bill);
                }
                
                else
                {
                    printf("Invalid customer type");
                }
            }
        }
        
        else
        {
            bill=20*units;
            printf("Your bill is %d",bill);
        }
    }
    
    return 0;      
        
}


TASK 3:
#include <stdio.h>

int main()
{
    int vehicleType, serviceType, hours, fee = 0;
    printf("Press 1 for Car\n");
    printf("Press 2 for Bike\n");
    printf("Press 3 for Bus\n");
scanf("%d", &vehicleType);

    printf("Enter number of hours: ");
scanf("%d", &hours);

    switch(vehicleType)
    {
        case 1:   // Car
            printf("Press 1 for Regular Parking (50 per hour)\n");
            printf("Press 2 for VIP Parking (100 per hour)\n");
            scanf("%d", &serviceType);

            switch(serviceType)
            {
                case 1:
                    fee = hours * 50;
                    break;
                case 2:
                    fee = hours * 100;
                    break;
                default:
                    printf("Invalid service type for Car\n");
            }
            break;

        case 2:   // Bike
            printf("Press 1 for Regular (20 per hour)\n");
            printf("Press 2 for Premium (40 per hour)\n");
            scanf("%d", &serviceType);

            switch(serviceType)
            {
                case 1:
                    fee = hours * 20;
                    break;
                case 2:
                    fee = hours * 40;
                    break;
                default:
                    printf("Invalid service type for Bike\n");
            }
            break;

        case 3:   // Bus
            fee = hours * 200;
            break;
        default:
            printf("Invalid vehicle type\n");
            return 0;
    }
    printf("Total parking fee = %d\n", fee);
    return 0;
}


TASK 4:
#include <stdio.h>

int main()
{
    int category, item, quantity;
    int price = 0, totalBill;
    printf("Press 1 for Fast Food\n");
    printf("Press 2 for Desi Food\n");
scanf("%d", &category);

    switch(category)
    {
        case 1:  
            printf("Press 1 for Burger (Rs. 500)\n");
            printf("Press 2 for Pizza (Rs. 1200)\n");
            scanf("%d", &item);

            switch(item)
            {
                case 1:
                    price = 500;
                    printf("You selected Burger\n");
                    break;
                case 2:
                    price = 1200;
                    printf("You selected Pizza\n");
                    break;
                default:
                    printf("Invalid Fast Food item\n");
                    return 0;
            }
            break;

        case 2:  
            printf("Press 1 for Biryani (Rs. 350)\n");
            printf("Press 2 for Karahi (Rs. 1500)\n");
            scanf("%d", &item);

            switch(item)
            {
                case 1:
                    price = 350;
                    printf("You selected Biryani\n");
                    break;
                case 2:
                    price = 1500;
                    printf("You selected Karahi\n");
                    break;
                default:
                    printf("Invalid Desi Food item\n");
                    return 0;
            }
            break;

        default:
            printf("Invalid category\n");
            return 0;
}

    printf("Enter quantity: ");
scanf("%d", &quantity);

totalBill = price * quantity;

printf("Total Bill = Rs. %d\n", totalBill);

    return 0;
}





TASK 5:
#include <stdio.h>

int main()
{
    float salary, bonus;
    int service;
    printf("Enter employee salary: ");
    scanf("%f", &salary);

    printf("Enter years of service: ");
    scanf("%d", &service);

    bonus = (service > 10) ? salary * 0.30 :
            (service > 5)  ? salary * 0.20 :
                             salary * 0.10;

    printf("Bonus amount = %.2f\n", bonus);

    return 0;
}



TASK 6:
#include <stdio.h>
int main() {
    float a, b, c;

    printf("Enter three sides of the triangle: ");
    scanf("%f %f %f", &a, &b, &c);


    if (a + b > c && a + c > b && b + c > a) {

        if (a == b && b == c) {
            printf("Equilateral Triangle\n");
        }

        else if (a == b || b == c || a == c) {
            printf("Isosceles Triangle\n");
        }

        else {
            printf("Scalene Triangle\n");
        }
    } else {

        printf("Not a valid triangle\n");
    }

    return 0;
}



TASK 7:
#include <stdio.h>
#include <string.h>

int main() {
    char username[20], password[20], otp[10];

    printf("Enter username: ");
    scanf("%s", username);

    if (strcmp(username, "6582") == 0) 
	{ 
        printf("Enter password: ");
        scanf("%s", password);

        if (strcmp(password, "1234") == 0) 
		{
            printf("Enter OTP: ");
            scanf("%s", otp);

            if (strcmp(otp, "4567") == 0) { 
                printf("Login Successful\n");
            } else {
                printf("Invalid OTP\n");
            }
        } 
		else 
		{
            printf("Incorrect Password\n");
        }
    } 
	else 
	{
        printf("Invalid Username\n");
    }

    return 0;
}

TASK 8:
#include <stdio.h>
#include <math.h>

int main() {
    int choice;
    double num1, num2, result;

    printf("Select operation:\n");
    printf("1 for Addition\n");
    printf("2 for Subtraction\n");
    printf("3 for Multiplication\n");
    printf("4 for Division\n");
    printf("5 for Square Root\n");
    printf("6 for Power (x^y)\n");
    printf("7 for Logarithm (log base 10)\n");
    printf("8 for Absolute Value\n");
    printf("9 for Sine\n");
    printf("10 for Cosine\n");
    printf("11 for Tangent\n");
    printf("Enter your choice: ");
    scanf("%d", &choice);

    switch(choice) {
        case 1:  
            printf("Enter first number: ");
            scanf("%lf", &num1);
            printf("Enter second number: ");
            scanf("%lf", &num2);
            result = num1 + num2;
            printf("Result = %.2lf\n", result);
            break;

        case 2: 
            printf("Enter first number: ");
            scanf("%lf", &num1);
            printf("Enter second number: ");
            scanf("%lf", &num2);
            result = num1 - num2;
            printf("Result = %.2lf\n", result);
            break;

        case 3: 
            printf("Enter first number: ");
            scanf("%lf", &num1);
            printf("Enter second number: ");
            scanf("%lf", &num2);
            result = num1 * num2;
            printf("Result = %.2lf\n", result);
            break;

        case 4: 
            printf("Enter numerator: ");
            scanf("%lf", &num1);
            printf("Enter denominator: ");
            scanf("%lf", &num2);
            if(num2 != 0)
                result = num1 / num2;
            else {
                printf("Error: Division by zero not allowed\n");
                break;
            }
            printf("Result = %.2lf\n", result);
            break;

        case 5:
            printf("Enter a number: ");
            scanf("%lf", &num1);
            if(num1 >= 0)
                result = sqrt(num1);
            else {
                printf("Error: Square root of negative number not allowed\n");
                break;
            }
            printf("Result = %.2lf\n", result);
            break;

        case 6: 
            printf("Enter base: ");
            scanf("%lf", &num1);
            printf("Enter exponent: ");
            scanf("%lf", &num2);
            result = pow(num1, num2);
            printf("Result = %.2lf\n", result);
            break;

        case 7: 
            printf("Enter a number: ");
            scanf("%lf", &num1);
            if(num1 > 0)
                result = log10(num1);
            else {
                printf("Error: Logarithm of zero or negative number not allowed\n");
                break;
            }
            printf("Result = %.2lf\n", result);
            break;

        case 8:
            printf("Enter a number: ");
            scanf("%lf", &num1);
            result = fabs(num1);
            printf("Result = %.2lf\n", result);
            break;

        case 9: 
            printf("Enter angle in radians: ");
            scanf("%lf", &num1);
            result = sin(num1);
            printf("Result = %.2lf\n", result);
            break;

        case 10: 
            printf("Enter angle in radians: ");
            scanf("%lf", &num1);
            result = cos(num1);
            printf("Result = %.2lf\n", result);
            break;

        case 11: 
            printf("Enter angle in radians: ");
            scanf("%lf", &num1);
            result = tan(num1);
            printf("Result = %.2lf\n", result);
            break;

        default:
            printf("Invalid operation\n");
    }
    return 0;
}

