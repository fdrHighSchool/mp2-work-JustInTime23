# Leap Year
#### Respond to the following:

1. Rewrite the following nested `if()` statements in a single line:
  ```
  if(year % 4 == 0 || year % 100 != 0 || year % 400 == 0) {
    isit = true;
  }
  else {
    isit = false;
    }
  return(isit);
  }
  ```

//2. Label each as either correct or incorrect syntax. If incorrect, rewrite below:
  * if (x == y) {

    //good

  * if [x == 10] {

    //NO if (x == 10) {

  * if x = 10 then {

    //NO if (x == 10) {

  * if (x equals 42) {

    //NO if (x == 42) {

  * if (x => y) {

    //NO (x >= y) {


3. Fix the error in the code below:

  ```
  Scanner console = new Scanner(System.in);
  System.out.print("What is your favorite color? ");
  String name = console.next();
  if (name == "blue") {
      System.out.println("Mine, too!");
  }
  ```

  * **YOUR WRITING HERE**
Scanner console = new Scanner(System.in);
  System.out.print("What is your favorite color? ");
  String name = console.nextLine();
  if (name.equals("blue")) {
      System.out.println("Mine, too!");
  }
