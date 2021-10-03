# -
перевод из 10 сс в любую меньше 10 сс
#include <iostream>
#include <string>
using namespace std;

int main()
{
    setlocale(0, "");
    int chislo,n,base;
    string st;
    cout << "Введите число и основание:" << endl;
    cin >> chislo >> base;
    int g;
    g = chislo;
    string mas;
    mas = "";
    while (chislo != 0){
        n = chislo % base;
        st = to_string(n);
        mas.append(st);
        chislo = chislo / base;
    }
    for (int i = mas.size(); i >= 0; i--) {
        cout << mas[i];
    }
}
