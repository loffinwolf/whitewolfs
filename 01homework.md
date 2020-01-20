### 과제_01homework

#### 노경준



1. Python에서 사용할 수 없는 식별자(예약어)를 찾아 작성하세요.

   > 파이썬에서 식별자는 변수, 함수, 모듈, 클래스 등을 식별하는데 사용되는 이름이다.
   >
   > - 보통 식별자의 이름은 영문알파벳, _, 숫자로 구성된다
   >
   > - 대소문자를 구분한다.
   >
   > - 아래의 예약어는 사용할 수 없다.
   >
   >   False, None, True, and, as, assert, break, class, continue, def, del, elif, else, except, finally, for, from, global, if, import, in, is, lamda, nonlocal, not, or, pass, raise, return, try, while, with, yield

2. 파이썬에서 float는 실수를 표현하는 과정에서 같은 값으로 일치되지 않습니다.

    (floating point rounding error) 따라서, 아래의 값을 비교하기 위해 작성해야하는 코드를 작성하세요. 

   

   `a = 0.1 * 3`

   ` b = 0.3`

   

   ```python
   import sys
   abs(a-b) <= sys.float_info.epsilon
   import math
   math.isclose(a, b)
   ```





3.  이스케이프 문자열 중 1) 줄바꿈 2) 탭 3) \ 을 작성하세요.

1) \n 2) \t 3)\\



4. “안녕, 철수야”를 String Interpolation을 사용하여 출력하세요

```python
`name = '철수'

print('"안녕, %s야"' %name)

print('"안녕, {}야"'.format(name))

print(f'"안녕, {name}야") 

 
```





5. 다음 중 형변환시 오류가 발생하는 것은?

   1) str(1)  2) int(‘30’)  3) int(5)  4) bool(‘50’)  5) int(‘3.5’)

   답 :  5번