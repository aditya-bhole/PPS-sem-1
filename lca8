#include <stdio.h>

int nearest(int *dist, int n) {
    int min = *dist;
    int i;
    for (i = 1; i < n; i++) {
        if (*(dist + i) < min) {
            min = *(dist + i);
        }
    }
    return min;
}

int main() {
    int n, dist[100], mindist, i;

    printf("Enter number of robots: ");
    scanf("%d", &n);

    printf("enter distance reading:\n");

    for (i = 0; i < n; i++) {
        printf("Sensor: ");
        scanf("%d", &dist[i]);
    }

    mindist = nearest(dist, n);

    printf("Nearest object= %d\n", mindist);

    if (mindist < 20) {
        printf("Warning");
    } else {
        printf("Path is clear");
    }

    return 0;
}
