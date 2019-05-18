# hello-world
Just One Repository


#include<stdio.h>
int main()
{
    int A, B, D, sum;
    scanf("%d %d %d", &A, &B, &D);
    sum = A + B;
    int num[100] = {0}, index = 0;

    do
    {
        num[index++] = sum % D;
        sum /= D;
    }while(sum != 0);

    for(int i = index - 1; i >= 0; i--)
        printf("%d", num[i]);

    return 0;
   /*
    long int A, B, num;
    int D, i = 0, a[100000] = {0};
    scanf("%ld %ld %d", &A, &B, &D);
    num = A + B;
    while(num != 0)
    {
        a[i++] = num % D;
        num /= D;
    }

    for(i--; i >= 0; i--)
        printf("%d", a[i]);
    
    return 0;
   */
}
