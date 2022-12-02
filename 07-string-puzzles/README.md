# String Puzzles
#### Respond to the following:

1. *In your own words*, discuss what each String method does:
  * `.substring(a)`
    * look at specific letter placement (indicated by a number starting at 0) and continue to the right

  * `.substring(a, b)`
    * look for a specific letter at point a

  * `.indexOf(str)`
    * Show amount of words in a string

  * `.equals(str)`
    * Way to compare strings with each other, as == does not work


2. *In your own words*, discuss what the following `for` loop accomplishes for `String s`:
```
for(int i = 0; i < s.length(); i++) {
      // DO STUFF
}
```
  * Repeats a process a specific amount of times, continue until i reaches the necessary quota and stop running the loop

class Main {
  public static void main(String[] args) {
    conCat("abc", "cat");
    firstHalf("WooHoo");
    repeatEnd("Hello", 3);
    countHi("hello hi"); //broken
    withoutString("Welcome stranger", "e");
    System.out.println("hi");
  }

  public static void withoutString(String sentence, String remove)  {
    System.out.println(sentence.replaceAll(remove, ""));
  }

  public static void countHi(String sentence) { //broken
    int check = 1;
    int amount = 0;
    while (check != -1) {
      check = sentence.indexOf("hi", 0);
      System.out.println(check);
      sentence.replaceFirst("hi", "");
      if (check != -1) {
        amount += 1;
      }
    }  
    System.out.println(amount);
  }
  // while (sentence.indexOf("hi", 0) != -1)

  public static void repeatEnd(String talk, int n) {
    int loop = n;
    while (loop != 0) {
      System.out.print(talk.substring(n-1 , talk.length()));
      loop -= 1;
    }
    System.out.println("");
  }

  public static void firstHalf(String word) {
    String print = word.substring(0, word.length()/2);
    System.out.println(print);
  }

  public static void conCat(String word1, String word2) {
    if (word1.substring(word1.length() - 1).equals(word2.substring(0,1))) {
      String new1 = word1.replace("c", "");
      System.out.println(new1 + word2);
    }
    else {
      System.out.println(word1 + word2);
    }
  }
}
