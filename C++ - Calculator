#include <cstdio> //timer
#include <ctime>  //timer
#include <iostream>

using namespace std;

class getCalc {

protected:
  double numOne, numTwo;
  double total;
  int getChoice;
  int delay; // timer

  int askDecide;

public:
  void calcStart() {
    choice();
    theChoice();
    askChoice();
  }

  void choice() {
    cout << "1)Add 2)Sub 3)Div 4) Mul \n" << endl;
    cin >> getChoice;
  }

  void askChoice() {
    cout << "1) Another operation? 2) Exit: ";
    cin >> askDecide;

    if (askDecide == 1) {
      cout << "GOING BACK TO THE MENU . . ." << endl;

      delay = 2;
      delay *= CLOCKS_PER_SEC;
      clock_t now = clock();
      while (clock() - now < delay)
        ;

      calcStart();
    }

    else if (askDecide == 2) {
      cout << "NOW EXITING CALCULATOR . . . " << endl;
      delay = 2;
      delay *= CLOCKS_PER_SEC;
      clock_t now = clock();
      while (clock() - now < delay)
        ;

      cout << "GOODBYE !" << endl;
    }
  }

  void theChoice() {
    switch (getChoice) {
    case 1:
      calcAdd();
      break;
    case 2:
      calcSub();
      break;
    case 3:
      calcDiv();
      break;
    case 4:
      calcMul();
      break;
    default:
      break;
    }
  }

  void calcAdd() {
    cout << "Enter first number to add: ";
    cin >> numOne;
    cout << "Enter second number to add "
         << "{" << numOne << "}"
         << " to: ";
    cin >> numTwo;
    total = numOne + numTwo;
    cout << numOne << " + " << numTwo << " = " << total << endl;
  }

  void calcSub() {
    cout << "Enter first number to sub: ";
    cin >> numOne;
    cout << "Enter second number to sub "
         << "{" << numOne << "}"
         << " from: ";
    cin >> numTwo;
    total = numOne - numTwo;
    cout << numOne << " - " << numTwo << " = " << total << endl;
  }

  void calcDiv() {
    cout << "Enter first number to Div: ";
    cin >> numOne;
    cout << "Enter second number to Div "
         << "{" << numOne << "}"
         << " from: ";
    cin >> numTwo;
    total = numOne / numTwo;
    cout << numOne << " / " << numTwo << " = " << total << endl;
  }
  void calcMul() {
    cout << "Enter first number to Mul: ";
    cin >> numOne;
    cout << "Enter second number to Mult "
         << "{" << numOne << "}"
         << " to: ";
    cin >> numTwo;
    total = numOne * numTwo;
    cout << numOne << " * " << numTwo << " = " << total << endl;
  }
};

int main() {

  getCalc CalculatorStart;

  CalculatorStart.calcStart();

  return 0;
}

