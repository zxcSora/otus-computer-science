#include <stdio.h>
#include <stdlib.h>
#include <time.h>


int main() {
    srand(time(NULL));
    int num_to_guess = rand() % 1000 + 1;
    int current_guess = 0;
    do {
        printf("Угадай число (1-1000): ");
        scanf("%d", &current_guess);
        if (current_guess == num_to_guess) {
            printf("АНО!!\n");
            break;
        } else {
            if (num_to_guess < current_guess) {
                printf("Больше\n");
            } else {
                printf("Меньше\n");
            }
        }
    } while (current_guess != num_to_guess);
    return 0;
}
