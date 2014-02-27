4digitprime
===========
#include <stdio.h>
#include <math.h>

int check(int);

int main(){
    int num, primeMax;
    for (num = 1000; num <= 9999; num++){
        if (check(num) == 1) primeMax = num;
        else continue;
        }
    printf("%d ga ichiban okiidesu", primeMax);
    return 0;
}

int check(int a){
    int factor, factorMax;
    factorMax = sqrt(a);
    for (factor = 2; factor <= factorMax; factor++){
        if (a%factor == 0) return 0;
        else continue;
        }
    return 1;
}
