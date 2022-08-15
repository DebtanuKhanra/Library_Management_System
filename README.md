# <p align="center"> Basic Notes on  <img width="70" height="30" src="https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white"></p>


 // this line of code is used to print something on display
 Console.WriteLine("Hello Wolrd");   
 
                               // DATA TYPE
/*

  Integer data type :  takes 4 bytes
         int a = 10;
  flaot data type :    takes 4 bytes
         float num = 1.23F;
  character data type : takes 2 bytes
         char c = 'A';
  Long data type : takes 8 bytes
         long number = 72615;
  Double data type : takes 8 bytes
         double num2 = 1.8276D;
  Boolean data type :    takes 1 bit
         bool isGreate = true;
                       = or false;
  String data type :    takes 2 bytes per character
         string name = "Istiaque"
             
  Note : one byte contains 8 bits
 */

  // example of datatypes :

   int a = 10;
   float b = 1.34F;
   double c = 1.34D;
   char s = 'E';
   bool isGreat = true;
   Console.WriteLine(a);
   Console.WriteLine(b);
   Console.WriteLine(c);
   Console.WriteLine(s);
   Console.WriteLine(isGreat);

                             // Take input from user 


  string name = Console.ReadLine();     // taking input from user and store the value into name
  Console.WriteLine(name);             //  this line of code display the user's input value


                            // Type Casting
/*
  Two types of type casting.
  1. Impicit Type casting 
     char to int to long to float to double  ( char value can be assigned/promoted in any of the datatype like int,long,float,double)
                                             ( int value can only be assigned/promote in long, float, double)
                                             ( long value can only be assigned/promote in float,double)
                                             ( float value can only be assigned/promote in double)

     int a = 10;
     double y = a;
     Console.WriteLine(y);     // this code is successfully run because int can be promoted into double.

     double y = 10;
     int a = y;
     Console.WriteLine(a);    // throws an error :  Cannot implicitly convert type `double' to `int'. An explicit conversion exists (are you missing a cast?)

   2. Explicit type casting
      
      int x =(int)3.4;       // double value is type casted into int and print the value of x is 3

  
   // We can also type cast using some methods.
    Convert.ToInt32();
    Convert.ToDouble();
    Convert.ToString();

    for example :
    
    a = 3.43;
    int a = Convert.ToInt32(3.43);
    Console.WriteLine(a);



                           --> How to take input from user-->

  // String input..

  Console.WriteLine("Enter your name : ");
  string name = Console.ReadLine();
  Console.WriteLine("Welcome to new world " + name);

  // Integer input..

  Console.Write("Enter the value of number1 :");
  int num1 = Convert.ToInt32(Console.ReadLine());
  Console.Write("Enter the value of number2 :");
  int num2 = Convert.ToInt32(Console.ReadLine());
  Console.WriteLine("Sum of " + num1 + " and " + num2 + " is :" + Convert.ToInt32(num1+num2));
         or
  Console.WriteLine("Sum of " + num1 + " and " + num2 + " is :" +(num1+num2));   -- We can also use "(num1+num2)" line .. using braket gives the priority


  --> Operators in C# -->
  
   1.Arithmatic Operator
   2.Assignment Operator
   3.Logical Operator
   4.Comparison Operator


 
                          --> Arithmatic Operator-->

  int a = 6;
  int b = 8;
  Console.WriteLine("The value of a + b is : " + (a+b));
  Console.WriteLine("The value of a - b is : " + (a-b));
  Console.WriteLine("The value of a / b is : " + (a/b));
  Console.WriteLine("The value of a * b is : " + (a*b));

                          --> Assignment Operator-->
 
  int a = 4;
      a += 4;
      a -= 4;
      a *= 4;
      a /= 4
  Console.WriteLine(a);


                          --> Logical Operator-->

  Console.WriteLine(true && false);
  Console.WriteLine(true && true);
  Console.WriteLine(false && false);

  Console.WriteLine(true || false);
  Console.WriteLine(true || true);
  Console.WriteLine(false || false);

  

  Console.WriteLine(!false);  -- not false mens true
  Console.WriteLine(!true);   --  not true means false


                           --> Comparator Operator-->

  Console.WriteLine(201>291);
  Console.WriteLine(201<=291);
  Console.WriteLine(201>=291);
  Console.WriteLine(201!=291);
  Console.WriteLine(201 ==201);



                           --> Math Function-->
  -- It takes 2 values inside the function and compares itselt and gives the result 

  int a = Math.Max(200,300);
  Console.WriteLine(a);

  int a = Math.Min(200,300);
  Console.WriteLine(a);

  int a = Math.Sqrt(36);      // throws an error becouse whenver we use sqrt function it return value in the double like Sqrt(39)
  Console.WriteLine(a);

  double a = Math.Sqrt(39);
  Console.WriteLine(a);



                                 --> String -->

  string name = "Hello Istiaque Ansari";
  Console.WriteLine(name.Length);                // Gives the length of string
  Console.WriteLine(name.ToUpper());            // Gives upper case of string
  Console.WriteLine(name.ToLower());           // Gives lower case of string

  string name = Console.ReadLine();
  string candies = Console.ReadLine();
  Console.WriteLine($"Your name is {name}. you will get {candies} candies");
 
  -- To make more readible we use above line of code coz it is not a good practice to use "+" every time to concatinate string


                 
                                           ---TO FIND THE CHARACTER using POSITION NUMBER---

string name= "DEBTANU CAZZZ";
Console.WriteLine(name[0]);   ---output= D
Console.WriteLine(name[1]);   ---output= E

                                              ---TO FIND THE INDEX NUMBER OF CHARCATER FROM A STRING---

string name= "DEBTANU CAZZZ VAI";
Console.WriteLine(name.IndexOf("CAZZZ"));  ---output= 8
Console.WriteLine(name.IndexOf("CAZZZ"));  ---output= 14

                              
                                    ---TO TAKE SUBSTRING FROM STARTING INDEX OF ANY POSITION OA A STRING---


string name= "DEBTANU CAZZZ VAI, ZINDEGI KHATAM HO GAYA APKA";
Console.WriteLine(name.Substring(14));				---output= VAI, ZINDEGI KHATAM HO GAYA APKA
Console.WriteLine(name.Substring(15));				---output= AI, ZINDEGI KHATAM HO GAYA APKA

string name= "DEBTANU CAZZZ VAI, \" ZINDEGI KHATAM HO GAYA APKA";
Console.WriteLine(name.Substring(15));				---output= AI, " ZINDEGI KHATAM HO GAYA APKA


  						
                                          ---SOME SPECIAL ESCAPE SEQUENCE CHARACTER CASE ---



The following is a list of defined C# escape sequences with corresponding representations:

\’ Single quotation mark used for character literals
\” Double quotation mark used for string literals
\\ Backslash used for file path
\? Question mark
\a Alert
\b Backspace
\f Form feed
\n New line
\r Carriage return
\t Horizontal tab
\v Vertical tab
\0 Null
\u Unicode escape sequence for a character with a hex value
\x Unicode hexadecimal escape sequence - similar to \u but with variable length
\U Unicode escape sequence used for surrogate pairs


                                                                     ---Some Basic Examples---

C#: P1

using  System;
class HelloWorld{
    static void Main(){
    
int age=Convert.ToInt32(Console.ReadLine());
if(age>18) {
    
     Console.WriteLine($"you are eligible to DRIVE");
}
else 
{
   Console.WriteLine("SORRY, YOU ARE NOT ELIGIBLE TO DRIVE");
}
  
}
}

INPUT: 12
OUTPUT: SORRY, YOU ARE NOT ELIGIBLE TO DRIVE






C#: P2 

using  System;
class HelloWorld{
    static void Main(){
        Console.Write("Enter your marks to check Status: ");
       int marks=int.Parse(Console.ReadLine());
       if(marks<=20){
           Console.WriteLine("FAIL, Concentrate on your studies");
       }
       else if(marks<=50){
           Console.WriteLine("PASS, but not a good marks");
       }
       else if(marks<=70){
           Console.WriteLine("very good");
       }
       else {
            Console.WriteLine("CONGRATULATIONS , YOU ARE TOPPER");
       }
}
}



INPUT: Enter your marks to check Status: 0
OUTPUT:FAIL, Concentrate on your studies





C#: P3 (Factorial of a number)

using  System;
class HelloWorld{
    static void Main(){
int number;
int fact =1;
int i;
Console.Write("Pleae Enter a Number: ");     
number=int.Parse(Console.ReadLine()); //Convert.ToInt32(Console.ReadLine());

for(i=1;i<=number;i++){
    fact=fact*i;
}
Console.Write($"The factorial of the {number} is {fact}");

}
}


INPUT:5
OUTPUT:120






C#: P4 (PALINDROME NUMBER PROGRAM)


using  System;
class HelloWorld{
    static void Main(){
        Console.Write("Enter the number: ");
        int number = int.Parse(Console.ReadLine());//Convert.ToInt32(Console.ReadLine());
        int rem;
        int temp;
        int result=0;
        
        temp=number;
        while(temp>0){
            rem=(temp%10);
            result=(result*10)+rem;
            temp=(temp/10);
        }
        if (result==number){
            Console.WriteLine($"WOW, {number} is a PALINDROME number");
        }
        else
        {
           Console.WriteLine( $"OOPS, {number} is not a PALINDROME number"); 
        }
}
}



INPUT: Enter the number: 15151
OUTPUT: WOW, 15151 is a PALINDROME number




C#: P5 (SWITCH CASE)


using  System;
class HelloWorld{
    static void Main(){
    Console.Write("Enter Your day: ");
   int day = int.Parse(Console.ReadLine());
   switch (day) {
  case 1:
    Console.WriteLine("Monday");
    break;
  case 2:
    Console.WriteLine("Tuesday");
    break;
  case 3:
    Console.WriteLine("Wednesday");
    break;
  case 4:
    Console.WriteLine("Thursday");
    break;
  case 5:
   Console.WriteLine("Friday");
    break;
  case 6:
    Console.WriteLine("Saturday");
    break;
  case 7:
    Console.WriteLine("Sunday");
    break;
  default:
    Console.WriteLine("You are illiterate, because only 7 days exist in a week");
    break;
}
}
}


INPUT: Enter Your day: 45
OUTPUT: You are illiterate, because only 7 days exist in a week




C#: P6 (CLASS AND OBJECT)

using System;

class david{
    public int age;
    public string name;
    public void cazz(){
       Console.WriteLine($" My name is {name} and i am {age} years old");
}


class HelloWorld {
  static void Main() {
    david n1= new david();
     Console.WriteLine("ENTER YOUR AGE: ");
    n1.age=int.Parse(Console.ReadLine());
    Console.WriteLine("ENTER YOUR name: ");
    n1.name=Console.ReadLine();
    n1.cazz();
    
  }
}


INPUT:ENTER YOUR AGE:
      98
      ENTER YOUR name: 
      debtanu
OUTPUT: My name is debtanu and i am 98 years old


















