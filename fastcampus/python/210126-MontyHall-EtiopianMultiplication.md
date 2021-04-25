# Etiopian multiplication

```
first_num = int(input('첫번째 숫자를 입력하세요: '))
second_num = int(input('두번째 숫자를 입력하세요: '))
nums = [first_num, second_num]
nums_lists = [[nums[0],nums[1]]]

while nums[0] !=1:
    nums[0] = nums[0] // 2
    nums[1] = nums[1] * 2
    nums_list = [nums[0],nums[1]]
    nums_lists.append(nums_list)

new_nums_lists = nums_lists[:]
for i in nums_lists:
    if i[0] % 2 == 0:
        new_nums_lists.remove(i)

nums_lists = new_nums_lists

result = 0
for i in nums_lists:
    result += i[1]

print('{0} 와 {1} 곱하기는 {2} 입니다.'.format(first_num, second_num, result))
```


# Monty Hall

```
import random
doors = [0, 0, 1]
random.shuffle(doors)
print('문 뒤:{}'.format(doors))
fir_q = int(input('3개의문 있습니다! 골라주세요~~~(1,2,3중에 고를것): ' )) - 1
door = doors[:]
door_index = [0, 1, 2]

if door[fir_q] == 1:
    door_index.remove(fir_q)
    print('다른방의 염소 위치는 {}번째 입니다.'.format(random.choice(door_index) + 1))
else:
    door[fir_q] = 1
    print('다른방의 염소 위치는 {} 번째 입니다.'.format(door.index(0) + 1))
    door[fir_q] = 0
print('바꾸면은 모든경우의 수 9가지중 6가지가 있기때문에 확률(66%)로는 좋습니다')
sec_q = input('바꾸시겠습니까?(yes or no): ')
if sec_q == 'yes':
    third_q = int(input('어디로 바꾸시겠습니까?(1, 2, 3중에 고르세요): ')) - 1
    if door[third_q] == 1:
        print('부릉부릉~~~')
    else:
        print('음메~~~')
elif sec_q == 'no':
    if door[fir_q] == 1:
        print('부릉부릉~~~')
    else:
        print('음메~~~')
else:
    print('yes or no!')
```
