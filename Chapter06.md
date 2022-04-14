**1. 다음은 C언어 코드이다. 출력 결과를 쓰시오.**

```C
#include <stdio.h>

void main( ){
   int i, j;
   int a[3][2] = {{1, 2}, {3, 4}, {5, 6}};
   int sum = 0;

   for(i=0; i<3; i++){
      for(j=0; j<2; j++){
          sum += a[i][j];
      }
   }

   printf("%.2f", (float)sum/(3*2));
}
```

<details>
<summary><b>정답 확인</b></summary>
<div markdown="1">

3.50

</div>
</details>
</br>

**2. 다음은 파이썬 프로그램이다. 실행결과를 쓰시오.**
```
li = ['Korea', 'America', 'China']
a=0
str01 = ''

for i in li:
   for j in i:
      str01 += j[0]
      a = a + 1
      if a > 5:
         break

print('a :', a, ', str01 :', str01)​
```
<details>
<summary><b>정답 확인</b></summary>
<div markdown="1">

a : 7, str01 : KoreaAC

</div>
</details>
</br>