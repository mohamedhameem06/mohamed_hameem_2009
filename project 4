#include <stdio.h>

struct students {
    int id;
    char name[50];
    int age;
    char city[50];
    float cutoff;
    char dob[20];
    char father_name[50];
    char mother_name[50];
};

int main() {
    struct students s1[10];
    
    for(int i = 0; i < 10; i++) {
        printf("\n Entering details for Student %d \n", i + 1);
        
        printf("Enter the student id: ");
        scanf("%d", &s1[i].id);
        
        printf("Enter student name: ");
        scanf("%s", s1[i].name);
        
        printf("Enter the age of the student: ");
        scanf("%d", &s1[i].age);
        
        printf("Enter your city: ");
        scanf("%s", s1[i].city);
        
        printf("Enter your cutoff: ");
        scanf("%f", &s1[i].cutoff);
        
        printf("Enter date of birth (DD/MM/YYYY): ");
        scanf("%s", s1[i].dob);
        
        printf("Enter father name: ");
        scanf("%s", s1[i].father_name);
        
        printf("Enter mother name: ");
        scanf("%s", s1[i].mother_name);
    }
    
    for(int i = 0; i < 10; i++) {
        printf("\nDetails for Student %d\n", i + 1);
        printf("ID: %d\n", s1[i].id);
        printf("Name:%s\n", s1[i].name);
        printf("Age:%d\n", s1[i].age);
        printf("City:%s\n", s1[i].city);
        printf("Cutoff:%d\n", s1[i].cutoff);
        printf("DOB:%s\n", s1[i].dob);
        printf("Father Name:%s\n", s1[i].father_name);
        printf("Mother Name:%s\n", s1[i].mother_name);
    }
    
    return 0;
}
