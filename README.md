#include <iostream>

int main() {
    double num1, num2;
    
    // Input dei due numeri
    std::cout << "Inserisci il primo numero: ";
    std::cin >> num1;
    
    std::cout << "Inserisci il secondo numero: ";
    std::cin >> num2;

    int scelta;
    std::cout << "Scegli l'ordine di visualizzazione:\n";
    std::cout << "1. Ordine crescente\n";
    std::cout << "2. Ordine decrescente\n";
    std::cout << "Inserisci la tua scelta (1 o 2): ";
    std::cin >> scelta;

    if (scelta == 1) {
        if (num1 < num2) {
            std::cout << "Numeri in ordine crescente: " << num1 << ", " << num2 << std::endl;
        } else {
            std::cout << "Numeri in ordine crescente: " << num2 << ", " << num1 << std::endl;
        }
    } else if (scelta == 2) {
        if (num1 > num2) {
            std::cout << "Numeri in ordine decrescente: " << num1 << ", " << num2 << std::endl;
        } else {
            std::cout << "Numeri in ordine decrescente: " << num2 << ", " << num1 << std::endl;
        }
    } else {
        std::cout << "Scelta non valida. Si prega di selezionare 1 o 2." << std::endl;
    }

    return 0;
}
