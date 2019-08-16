Test case : 1
Enter elements :                                                                                                                       
 arr[] : 1                                                                                                                             
 arr[] : 2                                                                                                                             
 arr[] : 3                                                                                                                             
 arr[] : 4                                                                                                                             
 arr[] : 5                                                                                                                             
                                                                                                                                       
Enter elements :                                                                                                                       
 arr[] : 1                                                                                                                             
 arr[] : 2                                                                                                                             
 arr[] : 3                                                                                                                             
 arr[] : 4                                                                                                                             
 arr[] : 5                                                                                                                             
Arrays are equal 



Test case : 2
Enter elements :                                                                                                                       
 arr[] : 1                                                                                                                             
 arr[] : 2                                                                                                                             
 arr[] : 3                                                                                                                             
 arr[] : 4                                                                                                                             
 arr[] : 5                                                                                                                             
                                                                                                                                       
Enter elements :                                                                                                                       
 arr[] : 2                                                                                                                             
 arr[] : 4                                                                                                                             
 arr[] : 6                                                                                                                             
 arr[] : 8                                                                                                                             
 arr[] : 1                                                                                                                             
Arrays are not equal 








#include <stdio.h>
void readArray(int arr[], int size) 
{ 
    int i =0; 
 
    printf("\nEnter elements : \n"); 
 
    for(i=0; i < size; i++) 
    { 
        printf(" arr[] : ",i); 
        scanf("%d",&arr[i]); 
    } 
} 
void printArray(int arr[],int size) 
{ 
    int i =0; 
 
    printf("\nElements are : "); 
 
    for(i=0; i < size; i++) 
    { 
        printf("\n\tarr[] : %d",i,arr[i]); 
    } 
    printf("/n");
}
char compareArray(int a[],int b[],int size)	{
	int i;
	for(i=0;i<size;i++){
		if(a[i]!=b[i])
			return 1;
	}
	return 0;
}

int main(){
	int a[5],b[5];
	readArray(a,5);
	readArray(b,5);
	
	if(compareArray(a,b,5)==0){
		printf("Arrays are equal\n");
		
	}
	else{
		printf("Arrays are not equal\n");
	}
		
	return 0;
}
