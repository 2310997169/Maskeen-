# Maskeen-2310997169
//In the field of programming, Iteration Statements are helpful when we need a specific task in repetition.
//They’re essential as they reduce hours of work to seconds. An iteration is a sequence of instructions that is
//continually repeated until a certain condition is reached. As per given statement you need to implement the
//task using iterations.
//A number is said to be valid if it is divisible by 8. Develop a logic that allows the user to keep entering
//numbers as long as the input is valid and also displays a count of the valid numbers.
#include <iostream>

int main() {
    int num, validCount = 0;
    bool validInput;

    do {
        std::cout << "Enter a number: ";
        std::cin >> num;
        validInput = std::cin && (num % 8 == 0);

        if (validInput) {
            validCount++;
            std::cout << "Valid number. Total valid numbers: " << validCount << std::endl;
        } else {
            std::cout << "Invalid number. Please enter a number divisible by 8." << std::endl;
        }
    } while (validInput);

    std::cout << "Exiting the program." << std::endl;

    return 0;
}
