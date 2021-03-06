Function(2) 숫자함수
=============

__1. round__  

  입력된 숫자를 반올림하여 출력. 옵션으로 반올림 자릿수를 설정함.  
  1은 소수점 아래 첫번째 자리까지 표시(두번째 자리에서 반올림), -1은 일의 자리에서 반올림하라는 의미.  
  MySQL은 오라클과 달리 FROM dual 로 가상테이블을 만들어줄 필요 없음. 생략 가능!
  
```
SELECT round(112.3456, 1), round(112.3456, 2), round(112.3456, -1) FROM dual;
```

<br/>

__2. truncate__

  round와 비슷하나, 반올림 대신 버림을 수행함.
  
```
SELECT truncate(112.3456, 1), truncate(112.3456, 2), truncate(112.3456, -1);
```

<br/>

__3. mod__

  첫번째 값을 두번째 값으로 나눈 나머지를 출력.
  
```
SELECT mod(26, 3), mod(10, 9), mod(4, 2);
```

<br/>

__4. ceil__

  입력된 숫자보다 크면서 가장 가까운 정수 출력.
  
```
SELECT ceil(12.6), ceil(11.5), ceil(16.3);
```

<br/>

__5. floor__

  입력된 숫자보다 작으면서 가장 가까운 정수 출력.

```
SELECT floor(12.6), floor(11.5), floor(16.3);
```

<br/>

__6. power__

  첫번째 값을 두번째 값만큼 제곱하여 출력.
  
```
SELECT power(1, 2), power(2, 3), power(3, 5);
```
