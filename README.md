#include <iostream>
#include <cmath>

int main() {
    double numero;

    // Input del numero
    std::cout << "Inserisci un numero: ";
    std::cin >> numero;

    // Verifica se il numero è non negativo prima di calcolare la radice quadrata
    if (numero >= 0) {
        double radiceQuadrata = std::sqrt(numero);
        std::cout << "La radice quadrata di " << numero << " è: " << radiceQuadrata << std::endl;
    } else {
        std::cout << "Errore: Impossibile calcolare la radice quadrata di un numero negativo." << std::endl;
    }

    return 0;
}

