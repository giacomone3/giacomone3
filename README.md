#include <iostream>

int main() {
    double consumoElettrico;
    double costoUnitario;
    double canoneFisso;

    // Input del consumo elettrico in kilowatt-ora
    std::cout << "Inserisci il consumo elettrico in kilowatt-ora: ";
    std::cin >> consumoElettrico;

    // Input del costo unitario per kilowatt-ora
    std::cout << "Inserisci il costo unitario per kilowatt-ora: ";
    std::cin >> costoUnitario;

    // Input dell'importo del canone fisso
    std::cout << "Inserisci l'importo del canone fisso: ";
    std::cin >> canoneFisso;

    // Calcola il costo totale della bolletta
    double costoConsumo = consumoElettrico * costoUnitario;
    double costoTotale = costoConsumo + canoneFisso;

    // Visualizza il costo totale della bolletta
    std::cout << "Il costo totale della bolletta è: " << costoTotale << " euro" << std::endl;

    return 0;
}


