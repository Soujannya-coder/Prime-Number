# Prime-Number

how to find a number is prime or not in c language :-

THE CODE IS -

#include <stdio.h>
int main() {
    int n, i, flag = 0;
    printf("Enter a positive integer: ");
    scanf("%d", &n);

    for (i = 2; i <= n / 2; ++i) {

        // condition for non-prime
        if (n % i == 0) {
            flag = 1;
            break;
        }
    }

    if (n == 1) {
        printf("1 is neither prime nor composite.");
    }
    else {
        if (flag == 0)
            printf("%d is a prime number.", n);
        else
            printf("%d is not a prime number.", n);
    }

    return 0;
}



#note - The smallest prime number is - 2
#note - The biggest prime number is - The largest known prime number is 2⁸² ⁵⁸⁹ ⁹³³ − 1, a number which has 24,862,048 digits when written in base 10. It was found via a computer volunteered by Patrick Laroche of the Great Internet Mersenne Prime Search in 2018. A prime number is a positive integer, excluding 1, with no divisors other than 1 and itself.
