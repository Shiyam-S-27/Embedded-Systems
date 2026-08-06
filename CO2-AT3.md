#include <stdio.h>

int main() {
    int sensor;

    printf("Industrial Fault Detection System\n");
    printf("Threshold Range: 50 - 200\n\n");

    printf("Enter sensor value: ");
    scanf("%d", &sensor);

    if (sensor < 50) {
        printf("Status: FAULT\n");
        printf("Reason: Value below minimum threshold.\n");
    }
    else if (sensor > 200) {
        printf("Status: FAULT\n");
        printf("Reason: Value above maximum threshold.\n");
    }
    else {
        printf("Status: NORMAL\n");
        printf("Sensor value is within the safe range.\n");
    }

    return 0;
}

