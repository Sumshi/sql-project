Write a program that prints the first 50 Fibonacci numbers, starting with 1 and 2, followed by a new line.The numbers must be separated by comma, followed by a space , 
You are allowed to use the standard library



#include <stdio.h>

int main(void) {
  unsigned long fib1 = 1;
  unsigned long fib2 = 2;
  int count;
  unsigned long current_fib;

  printf("%d, %d", 1, 2);
  for (count = 3; count <= 50; count++) {

     if ( count <= 50)
    {
      printf(", ");
    }
    current_fib = fib1 + fib2;
    printf("%lu", current_fib);
    fib1 = fib2;
    fib2 = current_fib;

    
  }
  printf("\n");
  return 0;
}
