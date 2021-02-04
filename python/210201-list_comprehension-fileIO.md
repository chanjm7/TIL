# Pytyon 06

## List Comprehension
```
old_list = [1, 2, 3, 4, 5,]

doubled_list = []
for i in old_list:
	doubled_list.append(i * 2)
```
```doubled_list = [i * 2 for i in old_list]  코드를 더 간결하게 만들수 있다```

### 만약 if문을 추가한다면
```doubled_list = [i * 2 for i in old_list if i % 2 == 0]```
- if문이 하나일땐 for문 뒤에 붙여준다
```
numbers = [1,2,3,4,5]
new_numbers = [item**2 if item%2==0 else item**3 for item in numbers]
```
- 두개 이상일땐 for문 앞에 붙여준다

## Dictionary Comprehension
```
numbers = [i for i in range(1,5+1)]
print(list(enumerate(numbers)))
```
- `enumerate` 순서가 있는 자료형의 순서와 값을 전달하는 기능이다 
```
old_dict = {1:1,2:2,3:3,4:4,}
new_dict = {}
for k,v in old_dict.items():
    if v%2!=0:
        new_dict[k*2]=v*3
```
```new_dict = {k*2:v*3 for k,v in old_dict.items() if v%2!=0}```
- 기존에 있던 딕셔너리를 이용해 새로운 딕셔너리를 만들때 코드를 더 간결하게 만들 수 있다

## File I/O
- `r` 읽기모드  `w` 쓰기모드  `a` 추가모드(파일의 마지막에 새로운 내용을 추가)
- `with open("파일이름", mode, encoding='utf-8') as f: f.write('입력할 내용')`
- `r` f.readline(), f.readlines()
- `.replace('찾을값, '바꿀값', 바꿀횟수)` 파일을 읽을때 정리할수있는 함수
- `a` 마지막에 enter한번 치고 나오기

### get(), setdefault()
- `get(key, default)` 키가 사전에 있으면 키 값을 반환하고 그렇지 않으면 기본값을 반환합니다. 기본값이 지정되지 않은 경우 기본값은 None이므로이 메서드는 KeyError를 발생시키지 않습니다.
- `setdefault(key, default)` 키가 사전에 있으면 해당 값을 반환합니다. 그렇지 않은 경우 기본값으로 키를 삽입하고 기본값을 반환합니다. 기본값은 없음입니다.
- 두개의 메소드는 키가 딕셔너리에 있을때 그 키의값을 주는건 같지만  없을경우에는 `get`은 default 값만 반환하지만 `setdefault`는 딕셔너리에 키와 default값을 삽입하고 default값을 반환한다.

### cvs, json
- `cvs`는 reader
`json`은 dump