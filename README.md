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
### TRIBONACCI SERIES
```c
#include <stdio.h>

int tribonacci(int n) {
    if(n==0){
        return 0;
    }
    if(n==1){
        return 1;
    }
    if(n==2){
        return 1;
    }
    return tribonacci(n-1) + tribonacci(n-2) + tribonacci(n-3);
}

int main(){
    int n;
    printf("Enter n: ");
    scanf("%d", &n);
    
    printf("%d\n", tribonacci(n));

    return 0;
}
```

# HACKERRANK RPOBELMS 
## PROBLEM:01

```c
#include <stdio.h>

struct student{
    char first_name[51] = {'j','o', 'h', 'n'};
    char last_name[51] = {'c','a','r','m','a','c','k'};
    int age = 15;
    int standard = 10;
}student;

int main() {
    
    printf("%d %s %s %d", student.age, student.first_name, student.last_name, student.standard);
    
    return 0;
}
```
