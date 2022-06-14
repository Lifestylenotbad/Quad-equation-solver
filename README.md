# Vot
#include <stdio.h>
#include <math.h>
int main()
{
	int d;
	float a, b, c, x1, x2, x;	
	printf("Чтобы найти корень Вашего уравнения введите коэффициенты a, b и c: \n");
	scanf("%f", &a); scanf("%f", &b); scanf("%f", &c);
	d = b * b - 4 * a * c;
    if(d > 0) {	x1 = (-b + sqrt(d)) / (2 * a);
	x2 = (-b - sqrt(d)) / (2 * a);
	printf("x1 = %f, x2 = %f", x1, x2);
	}
    if(d == 0) { x = -b / (2 * a);
	printf("x = %f", x);
	}
	if(d < 0) { printf("Нет корней");	
	}
getchar();
return 0;
}
