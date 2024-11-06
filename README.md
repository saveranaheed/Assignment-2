# Assignment-2
TASK 01:
```cpp
#include<iostream>
using namespace std;
int main() {
    double priceA=50.5;//price of product A
    double priceB=22.0;//price of product B
    double priceC=10.0;//price of product C
    int quantityA,quantityB,quantityC;
    std::cout<<"enter the quantity of product A:";
    std::cin>>quantityA;
    std::cout<<"enter the quantity of product B:";
    std::cin>>quantityB;
    std::cout<<"enter the quantity of product C:";
    std::cin>>quantityC;
    double total=(priceA*quantityA)+(priceB*quantityB)+(priceC*quantityC);
    std::cout<<"total cost:$"<<total<<std::endl;
    return 0;
}
```
OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/d97d9ba8-5822-43ca-8c11-d01e83a2ed03)

TASK#02:

```cpp
#include<iostream>
using namespace std;
int main() {
double priceA=30.0,priceB=20.0,priceC=10.0;
int quantityA, quantityB, quantityC;
cout<<"enter the quantity of product A:";
cin>>quantityA;
cout<<"enter the quantity of product B:";
cin>>quantityB;
cout<<"enter the quantity of product C:";
cin>>quantityC;
double total=(priceA*quantityA)+(priceB*quantityB)+(priceC*quantityC);
double finaltotal=(total>200)?total*0.9:total;
cout<<"total after discount:$"<<finaltotal<<endl;
return 0;
}
```
OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/98c59138-1cfd-41ca-9814-d16664ee69e1)

TASK#03:

```cpp
#include<iostream>
using namespace std;
int main() {
double priceA=50.0,priceB=30.0,priceC=20.0;
int quantityA,quantityB,quantityC;
cout<<"enter the quantity of product A:";
cin>>quantityA;
cout<<"enter the quantity of product B:";
cin>>quantityB;
cout<<"enter the quantity of product c:";
cin>>quantityC;
double total=(priceA * quantityA)+(priceB * quantityB)+(priceC * quantityC);
double finaltotal=(total>200)? 0.9 :total;
double shipping=(finaltotal<150)?15.0:0.0;
cout<<"total after discount and shipping:$"<<finaltotal+shipping<<endl;
return 0;
}
```

OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/7ea35170-8fa1-466f-ae90-4d5305a49aaa)

TASK#04:

```cpp
#include<iostream>
using namespace std;
int main() {
    double priceA = 50.0, priceB = 30.0, priceC = 20.0;
    int quantityA, quantityB, quantityC;
    cout << "Enter the quantity of Product A: ";
    cin >> quantityA;
    cout << "Enter the quantity of Product B: ";
    cin >> quantityB;
    cout << "Enter the quantity of Product C: ";
    cin >> quantityC;
    double total = (priceA*quantityA) + (priceB*quantityB) + (priceC*quantityC);
    double finalTotal = (total > 200) ? 0.9 : total;
    double shipping = (finalTotal < 150) ? 15.0 : 0.0;
    double totalWithShipping = finalTotal + shipping;
    int loyaltyPoints = (totalWithShipping > 300) ? 50 : 20;
    cout << "Total after discount and shipping: $" << totalWithShipping <<endl;
    cout << "Loyalty points earned: " << loyaltyPoints <<endl;
return 0;
}
```

OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/e8062f5d-a114-4d2e-bee1-573cab9eae17)


TASK#05

```cpp
#include<iostream>
using namespace std;
int main(){
int price1=45;
int price2=67;
int price3=29;
double quantity1=0;
double quantity2=0;
double quantity3=0;
cout<<"Enter the quantity for ProductA:";
cin>>quantity1;
cout<<"Enter the quantity for ProductB:";
cin>>quantity2;
cout<<"Enter the quantity for ProductC:";
cin>>quantity3;
double total=(price1*quantity1)+(price2*quantity2)+(price3*quantity3);
cout<<"Total:$"<<total<<endl;
double f_total=(total>200)?total*0.9:total;
cout<<"Total after discount:$"<<f_total<<endl;
double totalwithshipping=(f_total<150)?f_total+15.0:f_total;
cout<<"Total after discount and shipping:$"<<totalwithshipping<<endl;
int loyaltypoints=(totalwithshipping>300)?50:20;
cout<<"Loyalty points earned:"<<loyaltypoints<<endl;
return 0;
}
```

OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/af2dfcd6-a6d3-49d8-a51c-7bc2cdca934a)
