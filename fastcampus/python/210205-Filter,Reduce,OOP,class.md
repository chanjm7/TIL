# TIL08
## filter, reduce, OOP, class
- `filter`는 true or flase값만 보고 적용항다
`filter(함수, iterable)`
- `isinstance(비교할 값, 타입)` 타입이 맞으면 true 아니면 false
- `reduce(함수, 순회가능데이터, 초기값)` 여러개의 데이터를 대상으로 주로 누적 집계를 내기 위해 사용
### OOP
- 구현한 것을 드러나지 않도록 함
- 인터페이스로 클래스의 공통 특성을 묶어표현
- 자식 클래스가 부터 클래스의 특성과 기능을 물려받음
- 변수, method가 다른 상태를 가지는 것
### 구성요소
- class: 같은 종류의 집단에 속하는 속성과 행의의 정의
- object: class의 instance. 상위 class 의 속성과 함께 개별 특성과 method를 가짐
- method: 클래스로 생성된 객체의 사용법. 객체의 속성을 조작
