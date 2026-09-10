Parallel combination:
Total resistance:
Total current:
C Program
#include <stdio.h>

int main()
{
    float V, R1, R2, R3;
    float Rp, Rt, It, Vp, I1, I2, V3;

    printf("Enter supply voltage (V): ");
    scanf("%f", &V);

    printf("Enter R1, R2 and R3 values (ohms): ");
    scanf("%f %f %f", &R1, &R2, &R3);

    // R1 and R2 in parallel
    Rp = (R1 * R2) / (R1 + R2);

    // Total resistance
    Rt = Rp + R3;

    // Total current
    It = V / Rt;

    // Voltage across parallel combination
    Vp = It * Rp;

    // Currents through R1 and R2
    I1 = Vp / R1;
    I2 = Vp / R2;

    // Voltage across R3
    V3 = It * R3;

    printf("\nParallel Resistance = %.2f ohms", Rp);
    printf("\nTotal Resistance = %.2f ohms", Rt);
    printf("\nTotal Current = %.2f A", It);
    printf("\nVoltage across R1 and R2 = %.2f V", Vp);
    printf("\nCurrent through R1 = %.2f A", I1);
    printf("\nCurrent through R2 = %.2f A", I2);
    printf("\nVoltage across R3 = %.2f V", V3);

    return 0;
}
Example
For V = 12 V, R1 = 6 Ω, R2 = 3 Ω, R3 = 4 Ω:
Parallel resistance = 2 Ω
Total resistance = 6 Ω
Total current = 2 A
Voltage across R1 and R2 = 4 V
Current through R1 = 0.67 A
Current through R2 = 1.33 A
Voltage across R3 = 8 V# p-scal_.c
Calculation c program for parallel-series circuit
