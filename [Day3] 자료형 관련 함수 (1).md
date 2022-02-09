# 과제 리뷰

1. 조건문 예제 2개, 반복문 예제 2개, 조건문과 반복문을 모두 사용한 응용 예제 1개 만들어오기 (총 5개)

---

# 문자열, 리스트, 딕셔너리

> 문자열

각 요소에 인덱스로 접근할 수 있다.

```python
"자 이제 시작이야"
```

<br>

> 리스트

자료를 순서대로 저장한 구조다. 각 요소에 인덱스로 접근할 수 있다.

```python
["내", "꿈을", "위한", "여행"]
```

<br>

> 딕셔너리

Key-Value의 쌍으로 저장하며, Key는 중복될 수 없다. 각 요소에 Key로 접근할 수 있다.

```python
{"걱정" : "없음", "친구" : "있음"}
```

---

# 숫자형

> 나눗셈의 몫과 나머지

```python
5 % 3  # 2
```
```python
5 // 3  # 1
```
```python
divmod(5, 3)  # (1, 2)
```
<br>

> 연속된 정수

range 함수는 반복 가능(Iterable)한 객체를 반환하기 때문에 for문을 사용하여 출력해야 한다.

```python
range(10)  # 0~9 range(stop)
```
```python
range(1, 11)  # 1~10 range(start, stop)
```
```python
range(1, 11, 3)  # 1,4,7,10 range(start, stop, step)
```
```python
range(11, 1, -3)  # 11,8,5,2 range(start, stop, step)
```

---

# 문자열

> 따옴표 세개

```python
greet = """
Hi! I'm Sookyeong. Nice to meet you!
"""
```

<br>

> 인덱싱

```python
name = "Ponyo"
greet[0]  # "p"
greet[-1]  # "o"
```


<br>

> 슬라이싱

```python
name = "Ponyo"
name[1:]  # "onyo" name[start:]
name[:3]  # "Pon" name[:stop]
name[2:4] # "ny" name[start:stop]
name[:4:2]  # "pn" name[start:stop:step]
name[4:0:-2]  # "on" name[start:stop:step]
```

<br>

> 문자열의 연산

```python
last = "염"
first = "수경"
last + first  # "염수경"
first * 2  # "수경수경"
```

<br>

> 문자열의 길이

```python
long = "How long?"
len(long)  # 9
```

<br>

> 이스케이프 문자

```python
\n  # 개행
\t  # 탭
\  # 이스케이프
```

<br>

> 문자열 포맷팅

```python
fruit = "strawberry"
f"I like {fruit}"  # "I like strawberry"
"I like " + fruit  # "I like strawberry"

```

<br>

> 문자열 나누기

split 함수는 구분자를 기준으로 문자열을 나눠 리스트 형태로 반환한다.

```python
intro = "안녕하세요, 제 이름은 포뇨입니다."
intro.split()  # ['안녕하세요,', '제', '이름은', '포뇨입니다.']
intro.split(",")  # ['안녕하세요', ' 제 이름은 포뇨입니다.']
```

---

# 리스트

> 인덱싱

```python
todo = ["기상", "씻기", "밥"]
todo[1]  # ["씻기"]
todo[-1]  # ["밥"]
```

<br>

> 인덱스 찾기
```python
todo = ["기상", "씻기", "밥"]
todo.index("밥")  # 2
```

<br>

> 슬라이싱
```python
todo = ["기상", "씻기", "밥"]
todo[1:]  # ["씻기", "밥"]
```

<br>

> 리스트의 연산

```python
num = [1, 2, 3]
num2 = [4, 5, 6]
num + num2  # [1, 2, 3, 4, 5, 6]
num * 2  # [1, 2, 3, 1, 2, 3]
```

<br>

> 리스트의 길이
```python
todo = ["기상", "씻기", "밥"]
len(todo)  # 3
```

<br>

> 리스트 요소 추가

리스트의 마지막에 추가

```python
prev = []
prev.append("추가")
prev  # ["추가"]
---

특정 인덱스에 추가

```python
friend = ["피카츄", "파이리", "꼬부기"]
friend.insert(1, "라이츄")
friend  # ["피카츄", "라이츄", "파이리", "꼬부기"]
```

<br>

> 리스트 요소 제거

인덱스로 접근하여 제거

```python
friend = ["피카츄", "파이리", "꼬부기"]
del friend[0]
friend  # ["파이리", "꼬부기"]
```

Value로 접근하여 제거

```python
friend = ["피카츄", "파이리", "꼬부기"]
friend.remove("피카츄")
friend  # ["파이리", "꼬부기"]
```

인덱스 접근 + 인덱스 찾기 혼합

```python
friend = ["피카츄", "파이리", "꼬부기"]
del friend[friend.index("꼬부기")]
friend  # ["피카츄", "파이리"]
```

특정 요소 모두 제거

```python
num = [1, 2, 2, 2, 3, 4, 5, 6, 6]
while 2 in num:
    num.remove(2)
num  # [1, 3, 4, 5, 6, 6]
```

```python
ages = [22, 23, 24, 25, 25, 25, 26]
us = [22, 25]
age = [age for age in ages if age not in us]
age  # [23, 24, 26]
```

---

# 과제

1. 챌린지 도전
2. 자료형 관련 함수를 사용한 예제 3개 만들어오기
3. 각자 만들어보고 싶은 것 생각해오기
