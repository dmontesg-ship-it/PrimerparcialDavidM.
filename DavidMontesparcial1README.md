#include <iostream>
#include <iomanip>
using namespace std;

int main() {
    string nombre;
    double precio;
    int cantidad;
    double subtotal, iva, total;

    
    cout << "Ingrese el nombre del cliente: ";
    getline(cin, nombre);

    cout << "Ingrese el precio del producto: ";
    cin >> precio;

    cout << "Ingrese la cantidad comprada: ";
    cin >> cantidad;

    
    subtotal = precio * cantidad;
    iva = subtotal * 0.12;
    total = subtotal + iva;


    cout << fixed << setprecision(2);

    cout << "\n========= FACTURA =========" << endl;
    cout << "Cliente: " << nombre << endl;
    cout << "Subtotal: Q" << subtotal << endl;
    cout << "IVA (12%): Q" << iva << endl;
    cout << "Total a pagar: Q" << total << endl;

    return 0;
}
