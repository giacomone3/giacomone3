#include <iostream>

int main() {
    int larghezza, altezza;
    
    // Input della larghezza e altezza dell'immagine
    std::cout << "Inserisci la larghezza dell'immagine (in pixel): ";
    std::cin >> larghezza;
    
    std::cout << "Inserisci l'altezza dell'immagine (in pixel): ";
    std::cin >> altezza;

    // Calcola la dimensione in byte considerando 256 colori per pixel
    int dimensioneInByte = larghezza * altezza;

    // Verifica se l'immagine occupa più di 1 kbyte (1024 byte)
    if (dimensioneInByte > 1024) {
        std::cout << "L'immagine occupa più di 1 kilobyte." << std::endl;
    } else {
        std::cout << "L'immagine non occupa più di 1 kilobyte." << std::endl;
    }

    return 0;
}

