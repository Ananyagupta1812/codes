// C program for palindrom using iteratiion
#include <stdio.h>
int main()
{
    int n, m, p, sum = 0;
    printf("Enter any integer:");
    scanf("%d", &n);
    p = n;
    for (int i = 0; i <= n; i++)
    {
        m = n % 10;
        sum = (sum * 10) + m;
        n = n / 10;
    }
    printf("%d", sum);

    if (p == sum)
    {
        printf("\n%d is in palindrom", sum);
    }
    else
    {
        printf("\n%d is not in palindrom", sum);
    }
    return 0;
}
