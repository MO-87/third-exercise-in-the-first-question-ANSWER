# third-exercise-in-the-first-question-ANSWER

#include <stdio.h>

int main(){

int checker,m,n,k,num1,num2,num3;
    printf("Press 1 to print all the numbers divisible by k, for the the integers from m to n.\n");
    printf("Press 2 to read an integer from 1 to 999, and the print that integer in words.\n");
    printf("Press 0 to Exit program !!!\n");
    scanf("%d",&checker);

    if(checker==0)
        return 0;
    if(checker==1) {
        printf("Please enter k, m then n : ");
        scanf("%d%d%d", &k, &m, &n);
        for (int i = m; i <= n; ++i) {
            if (i % k == 0) { printf("%d ", i); }
        }
        return 0;
    }if(checker==2){
            printf("Please enter a number between 1 and 999 :");
            scanf("%d",&num1);
            printf("The number is ");
            if(num1/10>=10){
                num2=num1/10;
                if(num2/10==1)printf("One Hundred ");
                if(num2/10==2)printf("Two Hundred ");
                if(num2/10==3)printf("Three Hundred ");
                if(num2/10==4)printf("Four Hundred ");
                if(num2/10==5)printf("Five Hundred ");
                if(num2/10==6)printf("Six Hundred ");
                if(num2/10==7)printf("Seven Hundred ");
                if(num2/10==8)printf("Eight Hundred ");
                if(num2/10==9)printf("Nine Hundred ");
                if(num1%100>=10&&num1>=100){
                    num3=num1%100;
                    if(num3/10==1&&num1%10==0)printf("Ten ");
                    if(num3/10==2)printf("Twenty ");
                    if(num3/10==3)printf("Thirty ");
                    if(num3/10==4)printf("Forty ");
                    if(num3/10==5)printf("Fifty ");
                    if(num3/10==6)printf("Sixty ");
                    if(num3/10==7)printf("Seventy ");
                    if(num3/10==8)printf("Eighty ");
                    if(num3/10==9)printf("Ninety ");
                }if(num1%10>=1){
                    num3=num1%10;
                    if((num1/10)%10==1){
                        if(num3==1)printf("Eleven");
                        if(num3==2)printf("Twelve");
                        if(num3==3)printf("Thirteen");
                        if(num3==4)printf("Fourteen");
                        if(num3==5)printf("Fifteen");
                        if(num3==6)printf("Sixteen");
                        if(num3==7)printf("Seventeen");
                        if(num3==8)printf("Eighteen");
                        if(num3==9)printf("Nineteen");
                    }else {
                        if (num3 == 1)printf("One");
                        if (num3 == 2)printf("Two");
                        if (num3 == 3)printf("Three");
                        if (num3 == 4)printf("Four");
                        if (num3 == 5)printf("Five");
                        if (num3 == 6)printf("Six");
                        if (num3 == 7)printf("Seven");
                        if (num3 == 8)printf("Eight");
                        if (num3 == 9)printf("Nine");
                    }
                }
            }else if(num1/10<10&&num1>=10){
                if(num1/10==1&&num1%10==0)printf("Ten ");
                if(num1/10==2&&num1>=20)printf("Twenty ");
                if(num1/10==3&&num1>=20)printf("Thirty ");
                if(num1/10==4&&num1>=20)printf("Forty ");
                if(num1/10==5&&num1>=20)printf("Fifty ");
                if(num1/10==6&&num1>=20)printf("Sixty ");
                if(num1/10==7&&num1>=20)printf("Seventy ");
                if(num1/10==8&&num1>=20)printf("Eighty ");
                if(num1/10==9&&num1>=20)printf("Ninety ");
                if(num1%10>0){
                    if (num1%10==1&&num1>=20)printf("One");
                    if (num1%10==2&&num1>=20)printf("Two");
                    if (num1%10==3&&num1>=20)printf("Three");
                    if (num1%10==4&&num1>=20)printf("Four");
                    if (num1%10==5&&num1>=20)printf("Five");
                    if (num1%10==6&&num1>=20)printf("Six");
                    if (num1%10==7&&num1>=20)printf("Seven");
                    if (num1%10==8&&num1>=20)printf("Eight");
                    if (num1%10==9&&num1>=20)printf("Nine");
                    if(num1%10==1&&num1>10&&num1<20)printf("Eleven");
                    if(num1%10==2&&num1>10&&num1<20)printf("Twelve");
                    if(num1%10==3&&num1>10&&num1<20)printf("Thirteen");
                    if(num1%10==4&&num1>10&&num1<20)printf("Fourteen");
                    if(num1%10==5&&num1>10&&num1<20)printf("Fifteen");
                    if(num1%10==6&&num1>10&&num1<20)printf("Sixteen");
                    if(num1%10==7&&num1>10&&num1<20)printf("Seventeen");
                    if(num1%10==8&&num1>10&&num1<20)printf("Eighteen");
                    if(num1%10==9&&num1>10&&num1<20)printf("Nineteen");
                }
            }else {
                if (num1 == 1)printf("One");
                if (num1 == 2)printf("Two");
                if (num1 == 3)printf("Three");
                if (num1 == 4)printf("Four");
                if (num1 == 5)printf("Five");
                if (num1 == 6)printf("Six");
                if (num1 == 7)printf("Seven");
                if (num1 == 8)printf("Eight");
                if (num1 == 9)printf("Nine");
            }
        return 0;
    }
