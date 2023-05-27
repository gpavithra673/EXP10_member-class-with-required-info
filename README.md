# EXP10_member-class-with-required-info
## AIM:
### Create a class named 'Member' having the following members--
### Data members:
### 1 - Name
### 2 - Age
### 3 - Phone number
### 4 - Address
### 5 - Salary
### It also has a method named 'printSalary' which prints the salary of the members. Two classes 'Employee' and 'Manager' inherits the 'Member' class. The 'Employee' and 'Manager' classes have data members 'specialization' and 'department' respectively. Now, assign name, age, phone number, address and salary to an employee and a manager by making an object of both of these classes and print the same.
## PROCEDURE:
### 1.Create the class and declare the main method so that the JVM will identify the main program to run.
### 2.Create another class and use the keyword EXTENDS to use the concept of INHERITANCE.
### 3.Print a statement to check whether the inner class is accessable or not. 
### 4.If the extended class's statement is executed then,this program follows the concept of inheritance.
### 5.The program will be executed after the compilation and results are printed.
## PROGRAM:
```
package q2;

public class member {
    String []Name=new String[50];
    int []Age=new int[10];
    int []Phone=new int[10];
    String[] Addr =new String[50];
    int []Salary=new int[10];
    public void printSalary()
    {
        System.out.println("Salary: ");
    }
}

package q2;

public class Manager extends member{
    public void department(String dept){

        String Dept=dept;
    }
}
package q2;

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner sc= new Scanner(System.in);
        Employee emp= new Employee();
        for(int i=0;i<1;i++)
        {
            emp.Name[i]=sc.next();
            emp.Age[i]=sc.nextInt();
            emp.Phone[i]=sc.nextInt();
            emp.Addr[i]=sc.next();
            emp.Salary[i]=sc.nextInt();
        }
        System.out.println("Name         Age           Phone Number          Address          \t\tSalary");
        for(int i=0;i<1;i++)
        {
            System.out.println(emp.Name[i]+"\t\t"+"  "+emp.Age[i]+"\t\t\t"+emp.Phone[i]+"\t\t\t"+emp.Addr[i]+"\t\t\t"+emp.Salary[i]);
        }
    }
}
// CLASS 
package q2;

public class Employee extends member{
    public void specialisation()
    {
        System.out.println("Employee");
    }
}


```
