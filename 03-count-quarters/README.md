# Count Quarters
#### Respond to the following:

1. How do you isolate one-digit mkavkanasnkvava
* Make an indexOf() or length() dependent variable that only focuses on the "-1" part of the full number.

class Main {
  public static int countQuarters(int cents) {
    int numquarters;
    cents = cents % 100;
    if (cents.length() < 20) {
      numquarters = 0;
    }
    else {
      numquarters = cents/25;
    }
    return numquarters;
  }
}
