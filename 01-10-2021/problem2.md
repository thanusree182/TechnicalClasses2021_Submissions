/* Write a program to input an integer and output its octal equivalent 
(Hint: To obtain octal equivalent of an integer, divide it continuous by 8
 till dividend becomes zero, then write the remainders obtained in reverse direction.) */
 #include<stdio.h>
 int main() {
 	int a,i,j,b[30];
 	scanf("%d",&a);
 	while(a>0) {
 		b[i]=a%8;
 		a=a/8;
 		i++;
	 }
	 printf("Octal value:");
	 for(j=i-1;j>=0;j--) {
	 	printf("%d",b[j]);
	 }
	 return 0;
 }