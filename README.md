# The-uplift-project
A project of the Grilscript fountation.
Issue #1
#include<stdio.h>
  #include<stdlib.h>
  
  int main()
  {
  
   FILE *ptr;
   char c[100];

   ptr=fopen("test.txt","r");
   
   if(ptr==NULL)
   {
   	printf("the file is empty");
	   exit(1);
   }
    printf("enter the data");
    fgets(c,sizeof(c),stdin);
  
   	fprintf(ptr,"%s",c);
   
   fclose(ptr);
}
