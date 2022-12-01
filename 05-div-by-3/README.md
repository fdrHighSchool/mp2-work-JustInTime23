# Div By 3
#### Respond to the following:

1. A number is considered *prime* if its only factors are 1 and itself. For example, 7 is prime (1 and 7 are the only factors) and 9 is not (1, 3 and 9 are factors).  
Outline an algorithm to determine whether or not a number is prime.  
Think of the following method header:
`public static boolean isPrime(int num)`

  * class Main {
  public static void main(String[] args) {
    String initialNum = "9";
    int endNum = initialNum.indexOf(0);
    int result = 0;
    //continue to divide by continuously smaller digits w/ %, if index returns -1 (cannot find a number anymore) stop searching
    while (initialNum.indexOf(-1) != -1) {
      result += initialNum.charAt(-1);
      System.out.print(result);
    }
    /*
    int finalvalue1 = initialNum % 10;
    int finalvalue2 = initialNum % 1; 
    int grandfinale = finalvalue1 + finalvalue2;
    */
    boolean divby3;
    if (result % 3 == 0) {
      divby3 = true;
    }
    else {
      divby3 = false;
    }
    System.out.println(divby3);
  }
}
