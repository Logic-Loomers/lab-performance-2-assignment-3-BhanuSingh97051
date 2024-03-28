[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/Fmb6W2KK)
Design a C++ program for an employee payroll system. Create classes for Employee and Payroll. Users can add employees, enter hours worked, calculate salaries, and generate payroll reports.
#include <iostream>
#include <map>
#include <string>

int main() {
    std::map<std::string, std::string> bookMap;
    bookMap["9780132350884"] = "The C++ Programming Language";
    bookMap["9780321563842"] = "Effective C++";
    bookMap["9780201633610"] = "Design Patterns";
    std::string inputISBN;
    std::cout << "Enter the ISBN: ";
    std::cin >> inputISBN;
    auto bookIterator = bookMap.find(inputISBN);
    if (bookIterator != bookMap.end()) {
        std::cout << "Book Title: " << bookIterator->second << std::endl;
    } else {
        std::cout << "Book not available in the library." << std::endl;
    }

    return 0;
}
