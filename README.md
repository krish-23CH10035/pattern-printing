#include <stdio.h>

int main() {
  int i , j , rows ;
  char printChar ;
  scanf("%d",&rows);

  for(i = 0 ; i < rows ; i++){
    for(j = 0 ; j <( rows - i -1 ); j++) 
    printf(" ");
    printChar = 'A';

    for(j = 0 ; j <i ; j++){
      printf("%c",printChar);
      printChar =  printChar +1 ;
    }

    for(j =1 ; j<=2*i ; j++ ){
      printf("%c",printChar);
      printChar = printChar -1 ;
    }
    printf("\n");
  }
  return 0;
}
