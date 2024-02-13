//Write a program that prints the numbers from 1 to 100.For multiples of 3, print "Fizz"; for multiples of 5, print "Buzz"; and for numbers that are multiples of both 3 and 5, print "FizzBuzz".
function fizzBuzz(num) {
  console.log(num);
    for (var i = 0; i <= 100; i++) {
      if (i % 5 === 0 && i % 3 === 0 ) {
        console.log('fizzbuzz');
      } else if (i % 5 === 0) {
        console.log('buzz');
      } else if (i % 3 === 0) {
        console.log('fizz');
      } else {
        console.log(i);
      }
    }
  }

console.log(fizzBuzz(100));


//Write a program to generate the Fibonacci sequence up to 100
public class Fibonacci {
    // Don't check for negative number for simplicity
    public static int fibonacci(int n) {
        if (n < 2) {
            return n;
        } else {
            return fibonacci(n - 1) + fibonacci(n - 2);
        }
    }
 
    public static void main(String[] args) {
        int i = 0;
        int fn;
 
        while ((fn = fibonacci(i)) < 100) {
            System.out.print(fn + " ");
            i++;
        }
    }
}


//write a program that takes an integer as input and returns true if the input is a power of two.
#include <stdio.h>

//function prototype for checking power of two
int checkPowerofTwo(int n);

int main()
{
   int num;

   printf("Enter the number you want to test: ");
   scanf("%d", &num);

   if (checkPowerofTwo(num) == 1)
      printf("\n%d is a power of 2\n", num);
   else
      printf("\n%d is not a power of 2\n", num);

   return 0;
}

//function body
int checkPowerofTwo(int x)
{
   //checks whether a number is zero or not
   if (x == 0)
      return 0;

   //true till x is not equal to 1
   while( x != 1)
   {
      //checks whether a number is divisible by 2
      if(x % 2 != 0)
         return 0;
         x /= 2;
   }
   return 1;
}


//Write a program that accepts a string as input, capitalizes the first letter of each word in the string, and then returns the result string.
input_string = input("Enter a string: ")
result = capitalize_words(input_string)
print("Capitalized string:", result)


//Write a program that takes an integer as input and returns  an integer with reversed digit ordering.
def reverse_integer(num):
    # Check if the number is negative
    negative = False
    if num < 0:
        negative = True
        num = abs(num)
    
    # Convert the integer to a string and reverse it
    num_str = str(num)
    reversed_str = num_str[::-1]
    
    # Convert the reversed string back to an integer
    reversed_num = int(reversed_str)
    
    # If the original number was negative, make the reversed number negative
    if negative:
        reversed_num = -reversed_num
    
    return reversed_num

# Test the function
num = int(input("Enter an integer: "))
reversed_num = reverse_integer(num)
print("Reversed integer:", reversed_num)


//Write a program that counts the number of vowels in a sentence.
function countVowels(sentence) {
    // Convert the sentence to lowercase to simplify counting
    sentence = sentence.toLowerCase();
    
    // Define a list of vowels
    const vowels = ['a', 'e', 'i', 'o', 'u'];
    
    // Initialize a counter for vowels
    let vowelCount = 0;
    
    // Loop through each character in the sentence
    for (let char of sentence) {
        // If the character is a vowel, increment the count
        if (vowels.includes(char)) {
            vowelCount++;
        }
    }
    
    return vowelCount;
}
