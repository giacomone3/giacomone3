#include <iostream>

int main() {
    int nazionalita;

    // Input della nazionalità
    std::cout << "Inserisci il numero della tua nazionalità:\n";
    std::cout << "0 = italiano, 1 = inglese, 2 = francese\n";
    std::cout << "Scelta: ";
    std::cin >> nazionalita;

    // Comunica il saluto nella lingua corrispondente
    if (nazionalita == 0) {
        std::cout << "Ciao! Benvenuto!" << std::endl;
    } else if (nazionalita == 1) {
        std::cout << "Hello! Welcome!" << std::endl;
    } else if (nazionalita == 2) {
        std::cout << "Bonjour! Bienvenue!" << std::endl;
    } else {
        std::cout << "Nazionalità non riconosciuta. Per favore, inserisci 0, 1 o 2." << std::endl;
    }

    return 0;
}
