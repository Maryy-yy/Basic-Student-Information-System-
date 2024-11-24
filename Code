#include <iostream>

using namespace std;


const int max_students = 5;
const int grade_limit = 100;

string name, name1, name2, name3, name4, name5;
int age, age1, age2, age3, age4, age5;
float grade, grade1, grade2, grade3, grade4, grade5;
int student;
int studentCount = 0;
int choice;
float totalGrade;


int addStudent() {
    if (studentCount >= max_students) {
        cout << "Student limit reached. Cannot add more students." << endl;
        return studentCount;
    }

    cout << "Enter student name: ";
    cin >> name;

    cout << "Enter student age: ";
    cin >> age;

    do {
        cout << "Enter grade (0-100): ";
        cin >> grade;
        if (grade < 0 || grade > 100) {
            cout << "Invalid grade. Enter a grade between 0 and 100:" << endl;
        }
    } while (grade < 0 || grade > 100);

    if (studentCount==0){
        name1 = name;
        age1 = age;
        grade1 = grade;
    }
    else if (studentCount==1){
        name2 = name;
        age2 = age;
        grade2 = grade;
    }
    else if (studentCount==2){
        name3 = name;
        age3 = age;
        grade3 = grade;
    }
    else if (studentCount==3){
        name4 = name;
        age4 = age;
        grade4 = grade;
    }
    else if (studentCount==4){
        name5 = name;
        age5 = age;
        grade5 = grade;
    }

    cout << "Student Added Successfully! \n" << endl;
    studentCount++;
    return studentCount;
}

int viewStudents() {
        if (studentCount==0){
            cout << "No students to display."<< endl;
            return studentCount;
        }
        else {
            cout <<"List of Students: " << endl;
        if (studentCount>=1){
            cout << "1. Name: " <<name1 <<", Age: "<<age1<<", Grade: " <<grade1 << endl;
        }
        if (studentCount>=2){
            cout << "1. Name: " <<name2 <<", Age: "<<age2<<", Grade: " <<grade2 << endl;
        }
        if (studentCount>=3){
            cout << "1. Name: " <<name3 <<", Age: "<<age3<<", Grade: " <<grade3 << endl;
        }
        if (studentCount>=4){
            cout << "1. Name: " <<name4 <<", Age: "<<age4 <<", Grade: " <<grade4 << endl;
        }
        if (studentCount>=5){
            cout << "1. Name: " <<name5 <<", Age: "<<age5 <<", Grade: " <<grade5 << endl;
        }
    return studentCount;
}
}

float calculateAverageGrade() {
    if (studentCount == 0) {
        cout << "No students available to calculate the average grade." << endl;
        return 0.0;
    } else {
        float totalGrades = 0.0;
        if (studentCount >= 1) totalGrades += grade1;
        if (studentCount >= 2) totalGrades += grade2;
        if (studentCount >= 3) totalGrades += grade3;
        if (studentCount >= 4) totalGrades += grade4;
        if (studentCount == 5) totalGrades += grade5;

        float average = totalGrades / studentCount;
        return average;
    }
}

int main(){

    do {
        cout << "Student Information System" << endl;
        cout <<"1. Add Student" << endl;
        cout <<"2. View All Students" << endl;
        cout <<"3. Calculate Average Grade" << endl;
        cout <<"4. Exit" << endl;
        cout <<"Choose an option (1-4): ";
        cin >> choice;

        if (choice==1){
            addStudent();
        }
        else if (choice==2){
            viewStudents();
        }
        else if (choice == 3) {
            float average = calculateAverageGrade();
            if (average > 0) {
                cout << "The average grade is: " << average << endl;
            }
        }
        else if (choice==4){
            cout<<"Thank you for using the Student Information System!" ;
    }
} while (choice != 4);
    return 0;
}
