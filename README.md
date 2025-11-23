# leetCode.submission04

## PROBLEM:01
### CLIMING STAIRS

```c
#include <stdio.h>

int stair(int n){
    if(n==1) return 1;
    if(n==2) return 2;
    int ways = stair(n-1) + stair(n-2);
    return ways;
}

int main(){
    int n;
    printf("Enter number: ");
    scanf("%d", &n);
    printf("Number of ways: %d", stair(n));

    return 0;
}
```

## PROBELM:02
### FIBONACCI SERIES
```c
#include <stdio.h>

int fibonacci(int n){
    if(n<=2){
        return 1;
    }
    else{
        return fibonacci(n-1) + fibonacci(n-2);
    }
}

int main(){
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);
    printf("%d", fibonacci(n));
}
```
