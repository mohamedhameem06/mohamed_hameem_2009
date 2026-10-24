#include <stdio.h>
#include <string.h>

int main() {
    int balance = 1000;
    int password = 123;
    int user_password;
    int option;
    int user_amount;
    int user_depo;
    char isInsert[10];

    printf("Did you insert your card or not? ");
    scanf("%9s", isInsert);

    if (strcmp(isInsert, "yes") == 0) {

        printf("\n1. Balance Enquiry");
        printf("\n2. Withdraw");
        printf("\n3. Deposit");
        printf("\n4. Exit");

        printf("\nChoose any option (1, 2, 3, 4): ");
        scanf("%d", &option);

        switch (option) {

            case 1:
                printf("You chose the balance option\n");

                printf("Please enter your password: ");
                scanf("%d", &user_password);

                if (password == user_password) {
                    printf("Your bank balance is: %d\n", balance);
                } else {
                    printf("Wrong password!\n");
                }
                break;

            case 2:
                printf("You chose the withdrawal option\n");

                printf("Please enter your password: ");
                scanf("%d", &user_password);

                if (password == user_password) {

                    printf("How much amount do you want to withdraw? ");
                    scanf("%d", &user_amount);

                    if (user_amount > 0 && user_amount <= balance) {
                        balance = balance - user_amount;

                        printf("Withdrawal successful!\n");
                        printf("Remaining balance: %d\n", balance);
                    } else {
                        printf("Insufficient balance or invalid amount!\n");
                    }

                } else {
                    printf("Wrong password!\n");
                }
                break;

            case 3:
                printf("You chose the deposit option\n");

                printf("Please enter your password: ");
                scanf("%d", &user_password);

                if (user_password == password) {

                    printf("How much amount do you want to deposit? ");
                    scanf("%d", &user_depo);

                    if (user_depo > 0) {
                        balance = balance + user_depo;

                        printf("Amount deposited successfully!\n");
                        printf("Updated balance: %d\n", balance);
                    } else {
                        printf("Invalid deposit amount!\n");
                    }

                } else {
                    printf("Wrong password!\n");
                }
                break;

            case 4:
                printf("Thank you for using our ATM!\n");
                break;

            default:
                printf("Invalid option! Please choose between 1 and 4.\n");
        }

    } else {
        printf("Please insert your ATM card.\n");
    }

    return 0;
}
