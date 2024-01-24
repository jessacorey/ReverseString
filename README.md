#include <iostream>
#include <string>

// Function to reverse a string
std::string reverseString(const std::string& input) {
    return std::string(input.rbegin(), input.rend());
}

int main() {
    for (int i = 0; i < 3; ++i) {
        std::cout << "Enter a string: ";
        std::string userInput;
        
        // Read input with spaces
        std::getline(std::cin, userInput);

        // Reverse the string
        std::string reversedString = reverseString(userInput);

        // Print the reversed string
        std::cout << "Reversed string: " << reversedString << std::endl;
    }

    return 0;
}

