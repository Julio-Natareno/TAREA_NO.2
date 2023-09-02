#include <iostream>
using namespace std;

int main() {
    int numero;
    
   
    cout << "Ingrese un numero entero: ";
    cin >> numero;
    
   
    cout << "Elija en que posicion quiere el triangulo:" << endl;
    cout << "1. Triángulo  derecho" << endl;
    cout << "2. Triángulo  izquierdo" << endl;
    cout << "3. Triángulo  inferio" << endl;
    cout << "4. Triángulo  superior" << endl;
    int opcion;
    cin >> opcion;

   
    if (opcion >= 1 && opcion <= 4) {
        if (opcion == 1) {
            for (int i = 1; i <= numero; i++) {
                for (int j = 1; j <= i; j++) {
                    cout << "* ";
                }
                cout << endl;
            }
        } else if (opcion == 2) {
            for (int i = 1; i <= numero; i++) {
                for (int j = numero; j >= i; j--) {
                    cout << "* ";
                }
                cout << endl;
            }
        } else if (opcion == 3) {
            for (int i = 1; i <= numero; i++) {
                for (int j = 1; j <= numero - i; j++) {
                    cout << "  ";
                }
                for (int k = 1; k <= i; k++) {
                    cout << "* ";
                }
                cout << endl;
            }
        } else if (opcion == 4) {
            for (int i = 1; i <= numero; i++) {
                for (int j = 1; j <= i - 1; j++) {
                    cout << "  ";
                }
                for (int k = i; k <= numero; k++) {
                    cout << "* ";
                }
                cout << endl;
            }
        }
    } else {
        cout << "NO VALIDO." << endl;
    }

    return 0;
}