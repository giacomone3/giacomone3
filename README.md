#include <iostream>

int main() {
    int numeroStudenti;
    int numeroStudentiMenoDi15;
    double costoBiglietto;

    // Input del numero di studenti
    std::cout << "Inserisci il numero di studenti: ";
    std::cin >> numeroStudenti;

    // Input del numero di studenti con meno di 15 anni
    std::cout << "Inserisci il numero di studenti con meno di 15 anni: ";
    std::cin >> numeroStudentiMenoDi15;

    // Input del costo del biglietto
    std::cout << "Inserisci il costo del biglietto: ";
    std::cin >> costoBiglietto;

    // Calcola il numero di gruppi da 12 studenti con gratuità
    int gruppiConGratuita = numeroStudenti / 12;

    // Calcola il numero di studenti che non fanno parte di un gruppo da 12 studenti
    int studentiSenzaGratuita = numeroStudenti % 12;

    // Calcola l'importo totale con le gratuità
    double importoTotale = gruppiConGratuita * costoBiglietto * 11; // 11 biglietti pagati, 1 gratuito

    // Aggiungi l'importo per gli studenti rimanenti senza gratuità
    importoTotale += studentiSenzaGratuita * costoBiglietto;

    // Calcola lo sconto per gli studenti con meno di 15 anni
    double scontoStudentiMenoDi15 = costoBiglietto * 0.4 * numeroStudentiMenoDi15;

    // Sottrai lo sconto dall'importo totale
    importoTotale -= scontoStudentiMenoDi15;

    // Visualizza l'importo totale da pagare
    std::cout << "L'importo totale da pagare al cinema è: " << importoTotale << " euro" << std::endl;

    return 0;
}


