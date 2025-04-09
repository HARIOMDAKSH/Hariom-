 #include<Stdio.h>
#include"header.h"
int main(){
    printf("Enter number to check prime :- ");
    int n ;
    scanf("%d",&n);
    if(prime(n)==1){
        printf("Prime\n");
    }
    else{
        printf("Not prime\n");
    }

    printf("Enter number to check factorial :- ");
    int m ;
    scanf("%d",&m);
    printf("%d\n",factorial(m));

    printf("Enter number to check even/odd :-\n");
    int b ;
    scanf("%d",&b);
    if(evenodd(b)==0){
        printf("Even\n");
    }
    else{
        printf("Odd\n");
    }

}
[4/9, 8:19 AM] +91 93419 73440: int prime(int n){
    if(n==0 || n==1){
        return 0;
    for(int i =2;i<n;i++){
        if(n%i==0){
            return 0;
        }
    }
    return 1;
    }
}

int factorial(int m ){
    int product= 1;
    for(int i =1;i<=m;i++){
        product*=i;
    }
    return product;
}

int evenodd(int b){
    if(b%2==0){
        return 0;
    }
    return 1;
}
