#include <iostream>
#include <string>

class Employee {
private:
    std::string name;
    int employeeId;
    float salary;

public:
    Employee(std::string n, int id, float s) : name(n), employeeId(id), salary(s) {}

    void displayInfo() {
        std::cout << "Name: " << name << std::endl;
        std::cout << "Employee ID: " << employeeId << std::endl;
        std::cout << "Salary: " << salary << std::endl;
    }
};

int main() {
    Employee emp("John Doe", 12345, 50000);
    emp.displayInfo();

    return 0;
}
