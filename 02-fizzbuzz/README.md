# FizzBuzz
#### Respond to the following:

1. Fill out the following truth table:

| P  | Q  | P && Q | P \|\| Q |
|:--:|:--:|:------:|:--------:|
| T  | T  |   T    |    T     |
| T  | F  |   F    |    T     |
| F  | T  |   F    |    T     |
| F  | F  |   F    |    F     |


2. Prove a version of DeMorgan's Law:

| P  | Q  | P \|\| Q | ! (P \|\| Q) | !P | !Q | !P && !Q |
|:--:|:--:|:--------:|:------------:|:--:|:--:|:--------:|
| T  | T  |    F     |       F      | F  | F  |    F     |
| T  | F  |    F     |       F      | F  | T  |    F     |
| F  | T  |    F     |       F      | T  | F  |    F     |
| F  | F  |    T     |       T      | T  | T  |    T     |

3. What does DeMorgan's state and how did you prove it for the case above?
  * The inverse of OR is AND (and vice versa). This is proved when running a NOT or (and) or code (or NOT and [and] and code) and comparing the results.

class Main {
  public static void main(String[] args) {
    System.out.println("hard coded");
    double number = 15;
    if(number % 3 == 0) {
      System.out.print("Fizz");
    }
    if(number % 5 == 0) {
      System.out.print("Buzz");
    }
    if(number % 3 != 0 && number % 5 != 0) {
      System.out.println(number);
    }
  }
}
