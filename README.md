#include <iostream>

int main() {
    int numeroAlunni;
    const int costoBigliettoOrdinario = 12;
    const int numeroDocenti = 2;
    const double scontoDocente = 0.5; // 50% di sconto per i docenti

    // Input del numero di alunni
    std::cout << "Inserisci il numero di alunni: ";
    std::cin >> numeroAlunni;

    // Calcola il costo totale per gli alunni
    int costoAlunni = numeroAlunni * costoBigliettoOrdinario;

    // Calcola il costo totale per i docenti con sconto
    double costoDocenti = numeroDocenti * costoBigliettoOrdinario * (1 - scontoDocente);

    // Calcola il costo totale per l'intera scolaresca
    double costoTotale = costoAlunni + costoDocenti;

    // Visualizza il costo totale
    std::cout << "Il costo totale per la scolaresca è: " << costoTotale << " euro" << std::endl;

    return 0;
}

