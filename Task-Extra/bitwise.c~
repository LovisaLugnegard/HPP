#include<stdio.h>

typedef unsigned short n_type;

void print_bits(n_type a)
{
   int i;
   for(i = sizeof(n_type)*8; i > 0; i--)
      printf("%d", 1&(a >> i-1) );  

   printf("\n");
}

void count_bits(n_type bit){
   int i;
   int numBits = 0;
   for(i = sizeof(n_type)*8; i > 0; i--){
      if((1&(bit >> i-1)) == 1)
        numBits = numBits +1;
        }  
   printf("\n number of bits is: %d \n", numBits);      
}

int main(void){
   n_type a = 1123;
   n_type b = 3423;
   
   printf("a: \t");
   print_bits(a);
   count_bits(a);
   printf("b: \t");
   print_bits(b);
   count_bits(b);
   printf("a|b: \t");
   print_bits(a|b);
   count_bits(a|b);
   printf("a&b: \t");
   print_bits(a&b);
   count_bits(a&b);   
   printf("a^b: \t");
   print_bits(a^b);
   count_bits(a^b);   
   return 0;
}


