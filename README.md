#include <stdio.h>
int main()
{
   int num;
   FILE *fptr;

   if ((fptr = fopen("program.txt","r")) == NULL){
       printf("Error! opening file");

      
       exit(1);
   }

   fscanf(fptr,"%d", &num);

   printf("Value of n=%d\n", num);
   fclose(fptr); 
  
   return 0;
}
