#include <iostream>
using namespace std;

int main() {
    float monedas, precio, restante;

    cout << "Ingrese las monedas del jugador: ";
    cin >> monedas;

    cout << "Ingrese el precio del objeto: ";
    cin >> precio;

    if (monedas < 0 || precio < 0) {
        cout << "Error: los valores no pueden ser negativos." << endl;
    }
    else {
        if (monedas >= precio) {
            restante = monedas - precio;
            cout << "Compra exitosa." << endl;
            cout << "Monedas restantes: " << restante << endl;
        }
        else {
            cout << "Saldo insuficiente." << endl;
        }
    }

    return 0;
}

