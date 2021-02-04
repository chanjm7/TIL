# Python 07
### zip
`zip(iterable, iterable)`
- 동일한 개수로 이루어진 자료형을 묶어주는 역할을 하는 함수이다 개수가 차이가 나면 적은 자료형의 개수만 묶어주고 남은 값은 버린다

## Error Exception
```
try:
    pass
except:
    pass
```
- try에 실행문 except에 에러를 통해 할일
- 특정 에러를 정할수도 있다

## Regular Experssion
- 특정한 규칙을 가진 문자열의 집합을 표현하는데 사용하는 형식언어
- Python은 re모듈로 정규표현식 사용가능
- 외워서 하지말것
- `* asterick`는 0번째부터 `+`s는 1번째부터 주의하기
- `r`RegEx string이라는걸 알려준다
- RegEx를 쓸때 `complie()`을 하고 그 컴파일을 매치하는 식으로한다
## lambda
- 익명함수
- 간단한 수식을 함수로 지정해 한 두번 쓸 용도로 사용
- 두 줄 이상 실행될 함수는 그냥 함수로 정의
- Python은 모든 것이 객체로 존재
- 간단한 연산 함수도 객체로 존재하여 리소스를 점유
- 너무 남발해서 사용하지 않기
### map
- map(function, iterable)
- list의 각 element에 대해 특정한 함수를 적용
### filter
- filter(function, iterable)
- 특정함수를 만족하는 element만 남기는 필터

## 스택, 힙
### 스택
- 함수단위로 쌓는다
- 오래 쓰일것들을 스택에 쌓는다
### 힙
- 동적인 것들이 쌓여서 쓰이고 바로 지우고 자유롭게 늘었다 줄었다하는 제일 바쁜영역 lambda도 힙에 들어간다
- 한 두번 쓰일것들은 힙에 쌓는다
- 코드영역은 하드웨어에서 지우지 않는이상 계속 있는다
- 데이터영역은 실행되고 종료될때까지 쓰이는 영역

