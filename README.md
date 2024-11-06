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

Additional Task#01

```cpp
#include <iostream>
using namespace std;
int main() {
    double priceA = 50.0, priceB = 30.0, priceC = 20.0;
    int quantityA, quantityB, quantityC;
    double total, discount = 0.0, shipping = 5.0;
    int paymentMethod;
    cout << "Enter quantity for item A: ";
    cin >> quantityA;
    cout << "Enter quantity for item B: ";
    cin >> quantityB;
    cout << "Enter quantity for item C: ";
    cin >> quantityC;
    total = (priceA * quantityA) + (priceB * quantityB) + (priceC * quantityC);
    if (total > 100) {
        discount = total * 0.1; 
    }
    double totalWithShipping = total - discount + shipping;
    cout << "Select a payment method (1 for Credit Card, 2 for PayPal, 3 for Cash): ";
    cin >> paymentMethod;
    double transactionFee = 0.0;
    switch (paymentMethod) {
        case 1: 
            transactionFee = totalWithShipping * 0.02;
            break;
        case 2: 
            transactionFee = totalWithShipping * 0.03;
            break;
        case 3: 
            transactionFee = 0.0;
            break;
        default:
            cout << "Invalid payment method selected. Defaulting to Cash.\n";
            transactionFee = 0.0;
            break;
    }
    double totalAfterPayment = totalWithShipping + transactionFee;

    cout << "Total after applying transaction fee: $" << totalAfterPayment << std::endl;

    return 0;
}
```

OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/953314e3-f2e9-4b50-9864-c8584b5c8935)


Additional Task#02

```cpp
#include <iostream>
using namespace std;
int main() {
    double priceA = 50.0, priceB = 30.0, priceC = 20.0;
    int quantityA, quantityB, quantityC;
    int paymentMethod;
    cout << "Select a payment method (1 for Credit Card, 2 for PayPal, 3 for Cash): ";
    cin >> paymentMethod;
    double totalWithShipping = 0; 
    double transactionFee = 0;
    double totalAfterPayment = 0;  
    transactionFee = (paymentMethod == 1) ? totalWithShipping * 0.02 :
    (paymentMethod == 2) ? totalWithShipping * 0.03 : 0.0;
    totalAfterPayment = totalWithShipping + transactionFee;
    cout << "Total after applying transaction fee: $" << totalAfterPayment << endl;
    return 0;
}
```
OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/ed5cc116-dbd5-477e-8fe4-8f17e12acef5)

Additional Task#03:

```cpp
#include <iostream>
#include <string>
int main() {
    double finalAmount = 100.0; 
    std::string couponCode;
    std::cout << "Enter a coupon code (if any): ";
    std::cin >> couponCode;
    double couponDiscount = (couponCode == "SAVE10") ? 10.0 : 0.0;
  11
    double totalAfterCoupon = finalAmount - couponDiscount;
    std::cout << "Total after applying coupon: $" << totalAfterCoupon << std::endl;
    return 0;
}
```

OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/7d2f7576-63b5-4fc0-a688-0fee3a10bd3e)

Addition Task#04:

```cpp
#include <iostream>
using namespace std;
int main() {
    double finalAmount = 100.0; 
    int location;
    std::cout << "Enter your location (1, 2, or 3): ";
    std::cin >> location;
    double taxRate = (location == 1) ? 0.05 :      
     (location == 2) ? 0.10 :  0.08;             
    double totalWithTax = finalAmount * (1 + taxRate);
    std::cout << "Total after applying sales tax: $" << totalWithTax << std::endl;
    
    return 0;
}
```

OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/4e66fd1d-128d-4892-869c-16c9c206ffd4)


Additional Task#05

```cpp
#include <iostream>
using namespace std;
int main() {
  string productA = "Product A";
  string productB = "Product B";
  string productC = "Product C";
    double priceA = 10.0;  
    double priceB = 15.0;  
    double priceC = 20.0;
    int stockA = 10; 
    int stockB = 5;   
    int stockC = 8;  
    int quantityA, quantityB, quantityC;
    cout << "Enter quantity for " << productA << " (Available: " << stockA << "): ";
    cin >> quantityA;
    if (quantityA > stockA) {
        cout << "Sorry, only " << stockA << " units of " << productA << " are available.\n";
        quantityA = stockA; 
    }
    cout << "Enter quantity for " << productB << " (Available: " << stockB << "): ";
    cin >> quantityB;
    if (quantityB > stockB) {
        cout << "Sorry, only " << stockB << " units of " << productB << " are available.\n";
        quantityB = stockB;  
    }
    cout << "Enter quantity for " << productC << " (Available: " << stockC << "): ";
    cin >> quantityC;
    if (quantityC > stockC) {
    cout << "Sorry, only " << stockC << " units of " << productC << " are available.\n";
        quantityC = stockC; 
    }
    double subtotal = (priceA * quantityA) + (priceB * quantityB) + (priceC * quantityC);
    double discount = (subtotal > 50) ? subtotal * 0.10 : 0.0;
    double totalAfterDiscount = subtotal - discount;
    double shippingFee = (totalAfterDiscount > 100) ? 0.0 : 10.0;
    double taxRate = 0.08;
    double salesTax = totalAfterDiscount * taxRate;
    double finalTotal = totalAfterDiscount + salesTax + shippingFee;
    int loyaltyPoints = static_cast<int>(finalTotal / 5);
    cout << "\nOrder Summary:\n";
    cout << productA << " (x" << quantityA << "): $" << priceA * quantityA << endl;
    cout << productB << " (x" << quantityB << "): $" << priceB * quantityB << endl;
    cout << productC << " (x" << quantityC << "): $" << priceC * quantityC << endl;
    cout << "\nSubtotal: $" << subtotal << endl;
    cout << "Discount Applied: -$" << discount << endl;
    cout << "Shipping Fee: $" << shippingFee << endl;
    cout << "Sales Tax: $" << salesTax << std::endl;
   cout << "Total Amount to Pay: $" << finalTotal << endl;
    cout << "Loyalty Points Earned: " << loyaltyPoints << " points" << endl;
    return 0;
}
```
OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/9c53db6b-8b4d-4f99-9e36-8725adbc3064)

Additional Task#06:

```cpp
#include <iostream>
#include <string>
#include <iomanip>
int main() {
    std::string productA = "Product A";
    std::string productB = "Product B";
    std::string productC = "Product C";
    double priceA = 10.0;  
    double priceB = 15.0;
    double priceC = 20.0; 
    int stockA = 10;  
    int stockB = 5;   
    int stockC = 8;   
    int quantityA, quantityB, quantityC;
    std::cout << "Enter quantity for " << productA << " (Available: " << stockA << "): ";
    std::cin >> quantityA;
    if (quantityA > stockA) {
        std::cout << "Sorry, only " << stockA << " units of " << productA << " are available.\n";
        quantityA = stockA;  // Adjust the quantity to available stock
    }
    std::cout << "Enter quantity for " << productB << " (Available: " << stockB << "): ";
    std::cin >> quantityB;
    if (quantityB > stockB) {
        std::cout << "Sorry, only " << stockB << " units of " << productB << " are available.\n";
        quantityB = stockB;  // Adjust the quantity to available stock
    }
    std::cout << "Enter quantity for " << productC << " (Available: " << stockC << "): ";
    std::cin >> quantityC;
    
    if (quantityC > stockC) {
        std::cout << "Sorry, only " << stockC << " units of " << productC << " are available.\n";
        quantityC = stockC;  // Adjust the quantity to available stock
    }
    double subtotal = (priceA * quantityA) + (priceB * quantityB) + (priceC * quantityC);

    // Discount calculation (10% discount if subtotal is above $50)
    double discount = (subtotal > 50) ? subtotal * 0.10 : 0.0;
    double totalAfterDiscount = subtotal - discount;
    double shippingFee = (totalAfterDiscount > 100) ? 0.0 : 10.0;
    double taxRate = 0.08;
    double salesTax = totalAfterDiscount * taxRate;
    double finalTotal = totalAfterDiscount + salesTax + shippingFee;
    int loyaltyPoints = static_cast<int>(finalTotal / 5);
    std::cout << std::fixed << std::setprecision(2); // Setting precision for currency format
    std::cout << "\nOrder Summary:\n";
    std::cout << productA << " (x" << quantityA << "): $" << priceA * quantityA << std::endl;
    std::cout << productB << " (x" << quantityB << "): $" << priceB * quantityB << std::endl;
    std::cout << productC << " (x" << quantityC << "): $" << priceC * quantityC << std::endl;
    std::cout << "\nSubtotal: $" << subtotal << std::endl;
    std::cout << "Discount Applied: -$" << discount << std::endl;
    std::cout << "Shipping Fee: $" << shippingFee << std::endl;
    std::cout << "Sales Tax: $" << salesTax << std::endl;
    std::cout << "Total Amount to Pay: $" << finalTotal << std::endl;
    std::cout << "Loyalty Points Earned: " << loyaltyPoints << " points" << std::endl;
    return 0;
}
```
OUTPUT:

![Program
Output](https://github.com/user-attachments/assets/ba8a27e2-d382-449a-b6e6-398d42c6c1b2)


