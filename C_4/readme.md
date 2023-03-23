# 4주차 c언어 실습
  - 4주차 복습
  - 4주차 실습


~~~ c
#include <stdio.h>

int main(void)
{
    char code1= 'A';
    char code2= 65;

    printf("code1 = %c\n", code1);
    printf("code2 = %c\n", code2);
}
```


``` c
#include <stdio.h>

int main()
{
    double x, y, result;

    printf("두개의 실수를 입력하시오:");
    scanf("%lf %lf, &x, &y");

    result=x+y;
    printf("%f/%f=%f\n",x,y,result);

    result=x-y;
    printf("%f/%f=%f\n",x,y,result);

    result=x+y;
    printf("%f/%f=%f\n",x,y,result);

    result=x/y;
    printf("%f/%f=%f\n",x,y,result);

    return 0;
}
```

``` c
#include <stdio.h>

int main(void)
{
    int x=10, y=10;

    printf("x=%d\n",x);
    printf("++x의 값=%d\n",++x);
    printf("x=%d\n\n",x);

    printf("y=%d\n",y);
    printf("y++의 값=%d\n",y++);
    printf("y=%d\n",y);

    return 0;
}
```

``` c
#include <stdio.h>

int main(void)
{
    int money, change;
    int price, c5000,c1000,c500,c100,c10;

    printf("물건 값을 입력하시오:");
    scanf("%d", &price);
 
    printf("투입한 금액을 입력하시오:");
    scanf("%d",&money);
    change = money - price;

    c1000 = change / 1000;
    change = change % 1000;

    c500 = change / 500;
    change = change % 500;

    c100 = change / 100;
    change = change % 100;

    c10 = change / 10;
    change = change % 10;

    printf("\n천원권: %d장\n",c1000);
    printf("오백원 동전: %d개\n",c500);
    printf("백원 동전: %d\n",c100);
    printf("십원 동전: %d\n",c10);

    return 0;
}
```
