# 가상환경 설정, Decorator
## 가상환경 설정
### pyenv
- 버전관리
- pyenv activate 활성화
- pyenv deactivate 비활성화

### virtualenv
- 가상환경 관리

### poetry
- 패키지관리
- dependencies 실행에 관련된 라이브러리 장고
- dev-dependencies 개발에 관련된 로드테스트

## Decorator
- 함수를 받고 명령을 추가한 뒤 다시 함수형태로 반환하는 함수
- 함수 내부를 수정하지 않고 기능에 변화를 주고 싶을 때 사용
데코레이터 구조
```
def out_func(func):  # 기능을 추가할 함수를 인자로
    
    def inner_func(*args, **kwargs):

        return func(*args, **kwargs)
    
    return inner_func
```

## 느낀점
- 대충 가상환경을 좀 다뤄봤는데 정말 중요하다는걸 느꼈지만 아직 서투르다
- 장고수업 들어가면 제대로 다룰거 같으니 잘 알아두자
- decorator는 배우긴 했지만 잘 활용할지는 모르겠다