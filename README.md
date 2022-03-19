# Hafta8
Hafta 8 Ödevim


#include <iostream>
using namespace std;

class Kare {
private:     
float kenar;
public:
    void deger_atama(float);
    float cevre() {
        return 4 * kenar;
    }
    float alan() {
        return kenar * kenar;
    }
};

void Kare::deger_atama (float k) {
    kenar = k;
}

int main () {
    Kare kare1, kare2;
    kare1.deger_atama (6.2);
    kare2.deger_atama (4.3);

    cout<<"Kare 1 Cevresi: "<<kare1.cevre()<<" Alani: "<<kare1.alan()<<"\n";
    cout<<"Kare 2 Cevresi: "<<kare2.cevre()<<" Alani: "<<kare2.alan()<<"\n";

    return 0;
}
  
  
  
  
  
  
  #include <iostream>
using namespace std;

class Daire {
public:
    float yari_cap;
    float alan_bul(float yari_cap) {
        return 3.14 * yari_cap * yari_cap;
    }
};

int main () {
    Daire daire1, daire2;
    cout << "1. dairenin yaricapini giriniz: " ;
    cin >> daire1.yari_cap;

    cout << "2. dairenin yaricapini giriniz: " ;
    cin >> daire2.yari_cap;

    cout<<"Daire 1 Alani: "<<daire1.alan_bul(daire1.yari_cap)<<"\n";
    cout<<"Daire 2 Alani: "<<daire2.alan_bul(daire2.yari_cap)<<"\n";

    return 0;
}
