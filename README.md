# Siddharth.md
Here i will put the stuff that i want to access in future but for now it is not important for me 

## Exp 1-A  LED Flashing Code
#include <reg51.h>
#define Del 300

void delay(unsigned int time)
{
   unsigned int i, j;
   for(i = 0; i < time; i++)
      for(j = 0; j < 100; j++);
}

void main(void)
{
  while(1) {
    P1 = 0xFF;
    delay(300);
    P1 = 0x00;
    delay(300);
  }
}
