# Programas-en-c
codigos en c
// este programa calucula el complemento bianrio de un numero entre 0 y 255//
#include <stdio.h>
#include <math.h>
int main()
{
int A[8];
int k,j,i=0,m=0,b,posicion;

printf("Insert value from 0 to 255 =>");
scanf("%d",&b);
posicion = 0x80;

while(posicion != 0)
 {
 if((b & posicion) == 0)
 A[i] = 1;
  else
  A[i] = 0;
 posicion = posicion>>1;
 i++;
 }

for(j=0;j<=7;j++)
m = m + (A[j]*pow(2,7-j));
printf("El complemento binario de %d es %d \n",b,m);
}

