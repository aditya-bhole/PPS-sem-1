#include <stdio.h>
int main() {
    int i, j, r, c;
    printf("Enter the no of rows and columns: ");
    scanf("%d%d", &r, &c);
    int sen1[r][c], sen2[r][c], sen3[r][c];
    printf("Enter the first matrix:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            scanf("%d", &sen1[i][j]);
        }
    }
    printf("Enter the second matrix:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            scanf("%d", &sen2[i][j]); 
        }
    }
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            sen3[i][j] = sen1[i][j] + sen2[i][j];
        }
    }
    printf("The resultant matrix is:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            printf("%d \t", sen3[i][j]);
        }
            printf("\n");
    }
    return 0;
}
