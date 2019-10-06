#include <stdio.h>
#include <stdlib.h>

int main()
{
    int n,z,i;

    int h[]={0,0,0};
    long a[]={11111111,22222222,33333333},b[]={12121212,21212121,23232323},c[]={99999999,88888888,77777777};
    char d[3][15]={"agra", "ahmd", "lko"};
    char e[3][15]={"agra","lko","lko"};
    for(i=0;i<4;i++)
    {
        long l=0,k=0,s=0;
        printf("Enter the valid aadhar number,voter id card number and finger id\n");
        scanf("%ld %ld %ld",&l,&k,&s);
     int j;
     for(j=0;j<3;j++)
     {
         if(l==a[j]&&k==b[j]&&s==c[j])
         {h[j]++;
             if(h[j]<=1)
             {
             if(strcmp(d[j],e[j])==0)
             {
                 printf("1.BJP\n 2.CONGRESS\n 3.NOTA\n");
                 scanf("%d\n",&z);
             }
             else
             {
                printf("YOU ARE ELIGIBLE FOR VOTING FROM NEAREST City/Town/Village\n");
                printf("1.BJP\n 2.CONGRESS\n 3.NOTA\n");
                                 scanf("%d\n",&z);

                }
        }
             else
                {
                printf("Fake Voting\n");
             }
         }
        }
    }
    return 0;
}

