# Python04

## conditional Expressions
- `a`if`condition`else`b`
- `condition` == True=> a
- `condition` == False=> b
- ```'a' if 3<2 else 'b' if 4>3 else 'c' = 'b'```
- 연산자중 우선순위가 가장낮음

## for,While 반복문
- `break` 반복문을 끝낼때 사용
- `continue` 반복문을 스킵할때 사용

# for
- ```for i in range(int, int):
			출력문```
- ```range(이상, 미만)```

# while
- 조건 반복문
- `While True:`면은 무한loop

##FizzBuzz
- 1부터 100까지 반복할때 3의배수는 `Fizz`  5의배수는`Buzz` 15의 배수는 `FizzBuzz`
- 많이 반복되는  순서로 조건문을 쓰되 15배수가 뒤로가면 출력이 안되기 때문에 15배수는 예외로 맨앞에 놓고 그다음 3이 온다(리소스를 줄이기위해)
```for i in range(1, 100+1):
    if i % 15 == 0:
        print('i:{},FizzBuzz'.format(i))
    elif i % 3 == 0:
        print('i:{},Buzz'.format(i))
    elif i % 5 == 0:
        print('i:{},Fizz'.format(i))
    else:
        print('i:{}'.format(i))```


