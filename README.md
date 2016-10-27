# Stack

#include<stdio.h>

int push(int); 
int pop(int); 
int a[10];

int main(){
	int op,i, top = -1;
	printf("1. Insert \n 2. Delete \n");  
	printf("Enter the operation: \n"); 
	scanf("%d", &op);
	
	switch(op){
		case 1: push(top); 
		break; 
		case 2: pop(top); 
		break; 
		default: printf("Invalid Option"); 
		break; 
	}
	for(i=0; i<10; i++){
		printf("%d", &a[i]); 
	}
	return 0; 
}

int push(int top){
	if(top==10)
		printf("Full"); 
		return 0; 

	top++; 
	printf("Enter the element to be inserted");
	scanf("%d", &a[top]); 
	return 0; 
	}

int pop(int top){
	if(top==-1)
		printf("Empty"); 
		return 0; 
	a[top]=0; 
	top--; 
	return 0;
}



