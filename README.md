#include <iostream>

class BankAccount {
private:
    std::string accountNumber;
    float balance;

public:
    BankAccount(std::string accNum, float bal) : accountNumber(accNum), balance(bal) {}

    void deposit(float amount) {
        balance += amount;
    }

    void withdraw(float amount) {
        if (amount <= balance) {
            balance -= amount;
        } else {
            std::cout << "Insufficient balance!" << std::endl;
        }
    }

    void displayBalance() {
        std::cout << "Account Number: " << accountNumber << std::endl;
        std::cout << "Balance: " << balance << std::endl;
    }
};

int main() {
    BankAccount acc("123456789", 1000);
    acc.deposit(500);
    acc.withdraw(200);
    acc.displayBalance();

    return 0;
}
