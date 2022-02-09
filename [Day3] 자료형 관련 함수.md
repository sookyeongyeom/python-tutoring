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
greet[0]  # p
greet[-1]  # o
```


<br>

> 슬라이싱

```python
name = "Ponyo"
name[1:]  # onyo name[start:]
name[:3]  # Pon name[:stop]
name[2:4] # ny name[start:stop]
name[:4:2]  # pn name[start:stop:step]
name[4:0:-2]  # on name[start:stop:step]
```

<br>

> 문자열끼리의 연산

```python
last = "염"
first = "수경"
last + first  # 염수경
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
f"I like {fruit}"  # I like strawberry
"I like " + fruit  # I like strawberry

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



---

# if문

> 일치 확인

```python
country = input("Are you Korean?\n[1] Yes\n[2] No\n")

if country == "1":
    print("한국인이시구나~ㅎ")
elif country == "2":
    print("Umm... Bye.")
else:
    print("Please answer properly!")
```

<br>

> 불일치 확인

```python
answer = 25

guess = int(input("저 몇살이게요? : "))

if answer != guess:
    print("땡!")
else:
    print("눈썰미가 좋으시네!")
```

<br>

> 크기 비교

```python
money = input("돈 얼마 있어? : ")
money = int(money)

if money >= 7000:
    print("택시타고 가자!")
elif 5000 <= money < 7000:
    print("흠 좀 애매하네...")
else:
    print("걸어가자..ㅎ")
```

<br>

> 참/거짓 확인

```python
student = input("학생이신가요?\n[1] 네\n[2] 아니오\n")

if student == "1":
    is_student = True
else:
    is_student = False

if is_student == True:
    print("학생이시군요!")
else:
    print("학생이 아니시군요.")
```

<br>

> pass

```python
card = True

if card:
    pass
else:
    print("헉 카드 두고 왔어!")
```

---

# while문

> 기본

```python
while True:
    print("안녕?")
```

<br>

> 매 루프마다 1씩 더하기

```python
i = 0

while i < 10:
    print(f"i={i} | 아직 10 안됐음!")
    i += 1
```

<br>

> if문과 결합

```python
dabjeongneo = 2

while dabjeongneo != 1:
    dabjeongneo = input("1번이랑 2번 중에 뭐가 좋아? : ")
    if dabjeongneo == "1":
        print("흐흠 그럴 줄 알았어! *^-^*")
    else:
        pass
```

<br>

> break

```python
while True:
    dabjeongneo = input("1번이랑 2번 중에 뭐가 좋아? : ")
    if dabjeongneo == "1":
        print("흐흠 그럴 줄 알았어! *^-^*")
        break
    else:
        pass
```

<br>

> continue

```python
while True:
    dabjeongneo = input("1번이랑 2번 중에 뭐가 좋아? : ")
    if dabjeongneo != "1":
        continue
    else:
        print("흐흠 그럴 줄 알았어! *^-^*")
        break
```

---

# for문

> 기본

```python
for i in range(1, 11):
    print(i)
```

<br>

> 리스트 출력

```python
family = ["엄마", "아빠", "나", "동생"]

for member in family:
    print(member)
```

<br>

> 리스트 요소 평균값 구하기

```python
heights = [150, 160, 170, 180]
total = 0

for height in heights:
    total += height

print(f"평균 : {total/4}cm")
```

---

# 함수

> 기본

```python
def say():
    print("I'm saying!")

say()
```

<br>

> 매개변수 출력

```python
def greet(name):
    print(f"안녕하세요, {name}님!")

greet("포뇨")
```

<br>

> 매개변수 연산

```python
def number(a, b):
    print(f"a : {a}\nb : {b}")

number(1, 2)
number(b=3, a=1)
```

<br>

> 여러 개의 매개변수

```python
def call_names(*args):
    for name in args:
        print(name)

call_names("지윤", "궁", "포뇨", "수경")
```

<br>

> return

```python
def echo(text):
    return text

echo("안녕!")
print(echo("안녕!"))
```

<br>

> if문으로 return 알아보기

```python
def meockgeum(num):
    if num == 1:
        print("먹금합니다.")
        return
    else:
        print("먹금 실패!")
    print("이 부분이 출력될까요?")

meockgeum(1)
meockgeum(2)
```

---

# 응용 예제

> 네모의 여행

```bash
$ pip install keyboard
```

```python
import keyboard

white=" "
position = " ■"
print(position)
while True:
    if keyboard.read_key()=="d":
        white += " "
        print(white + position)
    elif keyboard.read_key()=="a":
        white = white.replace(" ","",1)
        print(white + position)
```

<br>

> 타이핑 효과

```python
import sys
import time

text = "안녕하세요..."

for letter in text:
    sys.stdout.write(letter)
    sys.stdout.flush()
    time.sleep(0.1)
```

---

# 자료형 별 특징 및 관련 함수 예시

> 숫자

```python
a = 1
```

1. 연산 가능 (+, -, *, /, %, //)

<br>

> 문자열

```python
a = "문자열입니다."
```

1. 큰따옴표, 작은따옴표, 큰따옴표3개
2. 이스케이프 (\n, \t, \\, \', \")
3. 연산 가능 (+, *)
4. 길이 구하기 (len)
5. 인덱싱
6. 슬라이싱
7. 문자열 포맷팅
8. 문자열 바꾸기 (replace)
9. 문자열 나누기 (split)

<br>

> 불

```python
a = True
b = False
```

1. 참/거짓
2. 빈 자료형 및 숫자 0 → False로 취급

<br>

> 리스트

```python
a = ["이런게", "리스트", "입니다"]
```

1. 인덱싱
2. 슬라이싱
3. 연산 가능 (+, *)
4. 길이 구하기 (len)
5. 수정/추가/삭제
6. 정렬 (sort)
7. 뒤집기 (reverse)

<br>

> 딕셔너리

```python
a = {"이름":"모찌", "성별":"남자", "나이":"5"}
```

1. Key-Value의 쌍으로, 순서 개념이 없다.
2. Key로 Value 얻기
3. 추가/삭제

---

# 과제

1. 챌린지 도전
2. 조건문 예제 2개, 반복문 예제 2개, 조건문과 반복문을 모두 사용한 응용 예제 1개 만들어오기 (총 5개)
