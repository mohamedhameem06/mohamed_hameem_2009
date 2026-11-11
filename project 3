#include <stdio.h>      // Header file for printf()
#include <stdlib.h>     // Header file for atoi()
#include <string.h>     // Header file for strcpy()

int main(int argc, char *argv[])  // Main function with command-line arguments
{
    int m1, m2, m3, m4, m5, total; // Declare integer variables for marks and total
    float average;                 // Declare float variable for average
    char name[30];                 // Declare character array to store student name

    if(argc != 7)                  // Check whether 7 arguments are given
    {
        printf("Usage: ./a.out Name M1 M2 M3 M4 M5\n");
                                     // Display usage instructions
        return 0;                    // Stop the program
    }

    strcpy(name, argv[1]);          // Copy student name into name variable

    m1 = atoi(argv[2]);             // Convert first mark into integer
    m2 = atoi(argv[3]);             // Convert second mark into integer
    m3 = atoi(argv[4]);             // Convert third mark into integer
    m4 = atoi(argv[5]);             // Convert fourth mark into integer
    m5 = atoi(argv[6]);             // Convert fifth mark into integer

    total = m1 + m2 + m3 + m4 + m5; // Calculate total of five marks
    average = total / 5.0;          // Calculate average of five marks

    printf("\n----- STUDENT REPORT -----\n"); // Print report heading
    printf("Student Name : %s\n", name);       // Display student name
    printf("Mark 1       : %d\n", m1);          // Display first mark
    printf("Mark 2       : %d\n", m2);          // Display second mark
    printf("Mark 3       : %d\n", m3);          // Display third mark
    printf("Mark 4       : %d\n", m4);          // Display fourth mark
    printf("Mark 5       : %d\n", m5);          // Display fifth mark

    printf("Total        : %d\n", total);       // Display total marks
    printf("Average      : %.2f\n", average);   // Display average to 2 decimals

    if(m1 < 35 || m2 < 35 || m3 < 35 ||
       m4 < 35 || m5 < 35)          // Check if any subject mark is below 35
    {
        printf("Result       : FAIL\n"); // Display FAIL
    }
    else
    {
        printf("Result       : PASS\n"); // Display PASS

        if(average >= 90)           // Check if average is 90 or above
            printf("Grade        : A+\n"); // Display A+ grade

        else if(average >= 80)      // Check if average is 80 or above
            printf("Grade        : A\n");  // Display A grade

        else if(average >= 70)      // Check if average is 70 or above
            printf("Grade        : B\n");  // Display B grade

        else if(average >= 60)      // Check if average is 60 or above
            printf("Grade        : C\n");  // Display C grade

        else                        // If average is below 60
            printf("Grade        : D\n");  // Display D grade
    }

    return 0;                       // End the program successfully
}
