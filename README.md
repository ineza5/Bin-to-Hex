#include <stdio.h>
#include <string.h>
#include <math.h>

void binaryToHexadecimal (const char *binary) {
    int decimal = 0;
    int length = strlen(binary);

    // Convert binary to decimal
    for (int i = 0; i < length; i++) {
        if (binary[length - 1 - i] = '1') {
            decimal += pow(2, i);
        }
}

    // Print the hexadecimal representation 
    printf ("Hexadecimal: %X\n", decimal);
}

int main() {
    char binary[65]; // 64 bits + 1 for null terminator

    printf("Enter a binary number: ");
    scanf("%64s", binary); // Read up to 64 characters 

    // Validate input 
    for (int i = 0; i <strlen(binary); i++) {
        if (binary[i] != '0' && binary[i] != '1') {
            print("Invalid binary number.\n");
            return 1;
        }
    }

    binaryToHexadecimal(binary);
    return 0;
}



# Bin-to-Hex
An assignment
