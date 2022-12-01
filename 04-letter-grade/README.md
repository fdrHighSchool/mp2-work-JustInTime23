# Letter Grade
#### Respond to the following:

1. Write a plan for the following extension:
  * Attach a "+" on their grade if the grade ends in a 7, 8 or 9 (eg: 78 -> C+, 89 -> B+)
  * Attach a "-" on their grade if the grade ends in a 0, 1 or 2 (eg: 92 -> A-, 61 -> D-)

    * class Main {
  public static void main(String[] args) {
    int g = 98;
    if (g >= 90) {
      System.out.println("A");
    }
    
    if (g >= 80 && g < 90) {
      System.out.println("B");
    }

    if (g >= 70 && g < 80) {
      System.out.println("C");
    }

    if (g >= 60 && g < 70) {
      System.out.println("D");
    }
    
    if (g < 60) {
      System.out.println("F");
    }

    if (g > 60) {
      String ja = String.valueOf(g);
      int check = ja.indexOf(0);
      if (check == 7 || check == 8 || check == 9 || g >= 100) {
        System.out.print("+");
      }
      
      if (check == 0 || check == 1 || check == 2) {
        System.out.print("-");
      }
    }
  } 
}



2. Discuss how you would make sure 100 is not misrepresented as an A-.
  * Modify the code to make an exception for 100 by not viewing the last digit of the grade, but seeing the grade as a whole instead.


3. Discuss how you would make sure grades that are an F are not mislabeled as F- or F+ (eg: 49 -> F+ and 52 -> F-)
  * Do not allow the + - code to run if the grade is less than 60.
