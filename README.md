# ALL-PF-LAB-TASKS 
#include <stdio.h>

TASK 5:
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
}


