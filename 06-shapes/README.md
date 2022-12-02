# Shapes
#### Respond to the following:

1. Write a plan for the following output:
```
000111222333444555666777888999
000111222333444555666777888999
000111222333444555666777888999
```
  * Print a fresh 0 int variable three times, add 1 every time that loop engages, println to a new line and repeat the process twice more


2. Write a plan for the following output:
```
999998888877777666665555544444333332222211111
999998888877777666665555544444333332222211111
999998888877777666665555544444333332222211111
999998888877777666665555544444333332222211111
999998888877777666665555544444333332222211111
```
  * Print a fresh 9 int variable three times, minus 1 every time that loop engages, println to a new line and repeat the process four times more

class Main {
  public static void main(String[] args) {
    //rectangle(3, 4);
     int  x = 3;
     int  y = 4;
    int staramount = x;
    while (y != 0) {
      while (staramount != 0){
      System.out.print("* ");
      staramount -= 1;
      }
    System.out.println("");
    staramount = x;
    y -= 1;
    }
    System.out.println("");
    
    int s = 3;
    
    for (int row = 0; row < s; row++) {
      for (int col = 0; col < s; col++) {
        System.out.print("* ");
      } // end col for loop
      System.out.println();
    } // end row for loop
    
  }
