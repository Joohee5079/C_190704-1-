# C_190704-1-
C_Class



#include <stdio.h>

int main()
{
    // 7개의 점수 중, 최대값 최솟값을 제외한 5개 정수의 평균을 구하시오.
  int i;
  float T, max, min, A;
	float S[] = {7.2, 3.8, 9.9, 9.8, 8.3, 9.1, 7.3};

	T = S[0];
	max = S[0];
	min = S[0];

    for (i = 1; i <= 6; i++)
    {
		if (max < S[i]) max = S[i];
		if (min > S[i]) min = S[i];
		T += S[i];
    }
	T = T - max - min;
	A = T / 5.0;
	printf("평균 : %f\n", A);
}
