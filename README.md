#include <stdio.h>
#include <time.h>

int main() {

	clock_t start, end;
	printf("ストップウォッチを開始します。\nEnterキーを押してください。");
	int c;
	c = getchar();
	putchar(c);
	start = clock();
	

	c = getchar();
	putchar(c);
	end = clock();
	printf("%.4f秒です。\n", (double)(end - start) / CLOCKS_PER_SEC);


	return 0;
}
