#include <stdio.h>
#include <string.h>

int checkLogin(char *login, char *passwd);
int checkValidPass(char *ps);

int main() {

    char login[64], password[64];

    printf("Enter login : ");
    scanf("%s", login);

    printf("Enter password : ");
    scanf("%s", password);

    if(checkLogin(login, password) == 1) {
        printf("Welcome\n");
    } else {
        printf("Incorrect login or password\n");
    }

    if(checkValidPass(password)) {
        printf("Accepted\n");
    } else {
        printf("Reject\n");
    }

    return 0;
}

int checkValidPass(char *ps) {

    int len = strlen(ps);
    int digit = 0;
    int upper = 0;
    int repeatUpper = 0;

    for(int i = 0; i < len; i++) {

        if(ps[i] >= '0' && ps[i] <= '9')
            digit++;

        if(ps[i] >= 'A' && ps[i] <= 'Z') {
            upper++;

            for(int j = i+1; j < len; j++) {
                if(ps[i] == ps[j])
                    repeatUpper = 1;
            }
        }
    }

    if(len == 5 && digit >= 1)
        return 1;

    if(len >= 5 && len <= 8 &&
       !(ps[0] >= '0' && ps[0] <= '9') &&
       upper >= 2 &&
       digit >= 2)
        return 1;

    if(len >= 5 && len <= 8 &&
       upper >= 2 &&
       digit >= 2 &&
       repeatUpper == 0)
        return 1;

    return 0;
}

int checkLogin(char *login, char *passwd) {

    if(!strcmp(login, "student1") &&
       !strcmp(passwd, "mypass"))
        return 1;
    else
        return 0;
}
