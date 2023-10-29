#include <iostream>

int main() {
    double saldoEuro;
    
    // Input del saldo del conto corrente in euro
    std::cout << "Inserisci il saldo del conto corrente in euro: ";
    std::cin >> saldoEuro;

    // Tassi di cambio più recenti (da euro a yen e da euro a dollari)
    double tassoCambioEuroToYen = 127.0;    // 1 euro = 127 yen (esempio)
    double tassoCambioEuroToDollari = 1.15; // 1 euro = 1.15 dollari (esempio)

    // Calcola il saldo in yen e dollari
    double saldoYen = saldoEuro * tassoCambioEuroToYen;
    double saldoDollari = saldoEuro * tassoCambioEuroToDollari;

    // Individua la relazione tra yen e dollari
    double rapportoYenDollari = saldoYen / saldoDollari;

    // Visualizza il saldo in yen e dollari, e il rapporto
    std::cout << "Saldo in yen: " << saldoYen << " yen" << std::endl;
    std::cout << "Saldo in dollari: " << saldoDollari << " dollari" << std::endl;
    std::cout << "Rapporto tra yen e dollari: 1 euro = " << rapportoYenDollari << " yen" << std::endl;

    return 0;
}

