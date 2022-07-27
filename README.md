# Solution-of-CSE-103-Lab-Test
The solution of CSE 103 Lab Test at 27 July 2022                

Solution of Problem 1                                           #1

Input  =    7  >>  Output = 1.625118
Input  =  13.5 >>  Output = 1.109740

The code of Problem 1
[[ You can use double instead of float ]]

#include<stdio.h>
#include<math.h>

int main()

{
    float x,y,z,s,c;

    printf("Enter a numeric number:");
    scanf("%f",&x);

    z = sqrt(2);
    s = sin(x/3);
    c = 3 + ((cos(x))*(cos(x))*(cos(x)));
    y = z + (s/c);

    printf("%f\n",y);

    return 0;
}

The code is end.

Solution of Problem 2                                           #2

Input = 10001 >> Output = 0
Input = 27763 >> Output = 8 

The code of Problem 2
[[ You can use any data type without character ]]

#include<stdio.h>
#include<math.h>

int main()

{
    int i, n, digit, sum = 0;

    scanf("%d",&n);

    for(i=n;i>0;i=i/10)
    {
        digit=i%10;
        if(digit%2==0)
        {
            sum = sum+digit;
        }
    }

    printf("%d",sum);

    return 0;
}

The code is end.

Solution of Problem 3                                           #3

Input = 5 >> Output = 1+(-2)+3+(-4)+5 = 3
Input = 3 >> Output = 1+(-2)+3        = 2

The code of Problem 3

#include<stdio.h>
#include<math.h>

int main()

{
    int n,i,sum = 0;
    scanf("%d",&n);

    for(i=1;i<=n;i++)
    {
        if(i%2!=0)
        {
            printf("%d",i);
            if(i<n)
            {
                printf("+");
            }
            sum = sum + i;
        }
        else
        {
            printf("(-%d)+",i);
        }
    }

    printf(" = %d",sum);

    return 0;
}

Solution of Problem 4                                           #4

The code of Problem 4

#include<stdio.h>
int main()

{
    int a, b, n, inc = 0, dec = 0;

    scanf("%d",&n);

    for(int i = 0 ; i < n ; i++)
    {
        if(i>0) b = a;
        scanf("%d", &a);
        if(i == 0)
        {
            inc++ ;
            dec++ ;
        }
        else{
            if(a>b) inc++;
            else dec++ ;
        }
    }

    if(inc == n || dec == n) printf("Ordered\n");
    else printf("Not Ordered\n");

}


                                                                  The End.
