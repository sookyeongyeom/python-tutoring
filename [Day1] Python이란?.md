# Python이란?

## 1. 프로그래밍 언어란?
인간(Hello World!) ⇔ 프로그래밍 언어 ⇔ 컴퓨터(0110101...)   
프로그래밍 언어는 한두개가 아니다.   
그러나 작동 기전이 비슷하기 때문에 전체적인 메커니즘을 알게 되면 새로운 언어도 익히기 쉽다.

## 2. 프로그래밍 언어는 메모장에 적어도 작동한다.
메모장에 코드를 작성 후 확장자를 바꿔주면 프로그램으로서 기능할 수 있다.   
근본적으로 코드는 메모장에 써도 작동하지만, 보조를 받아 편하게 쓰기 위해 에디터를 사용한다. (자동완성, 맞춤법 검사 등)   
이런 에디터들을 IDE(Integrated Development Environment)라고 부른다.

## 3. 왜 Python인가?
Python은 짧다.   
High Level에 가까울수록 성능은 떨어지지만 개발 속도는 월등히 빨라진다.   
Python으로 작성된 상용 라이브러리는 매우 많다.   
알고리즘 문제 풀이 위주의 강의는 초심자의 기를 쉽게 꺾는다.   
스스로 만들고 싶은 프로그램을 만들어보며 공부할 수 있기 때문에 첫 입문으로는 Python을 추천한다.   
또한, Python은 쉽다고해서 '부족한' 언어가 아니다.   
시스템과 밀접한 영역이나 모바일 프로그래밍을 제외하면 모든 영역에서 Python은 사용될 수 있다.   

## 4. High Level?
인간의 언어와 가까운 문법을 가진 언어를 말한다.   
Python으로 하는 개발은 마치 컴퓨터와 영어로 대화하는 듯한 느낌을 준다.   

---

# Python 및 Editor 설치

## 1. Python 설치
Mac https://blockdmask.tistory.com/341   
Windows10 https://goddaehee.tistory.com/286   
### 대화형 Interpreter (cmd/terminal)
Python은 한 줄 한 줄 순차적으로 실행된다.   
cmd/terminal에서 Python의 대화형 인터프리터를 실행할 수 있다. 
1. 사칙연산
2. 변수에 숫자 대입하고 계산하기
3. 변수에 문자 대입하고 출력하기

## 2. VSCode 설치
Mac https://eunoia3jy.tistory.com/92   
Windows10 https://www.lainyzine.com/ko/article/how-to-install-visual-studio-code-on-windows-10/   
### VSCode란?
VSCode는 Python 전용 Editor는 아니다.   
사용가능한 언어에 제한이 없다.   
가볍고 구동이 빨라 선호된다.   
### VSCode 사용방법 설명
1. 폴더 열기   
2. Extension (Python, Black)  
3. Terminal    

---

# Python 맛보기

## 1. 문자열 출력

```python
print("Hello World!")
```

C/Unix의 개발자가 집필한 C교재의 첫 예제에서 유래했다.   

## 2. 문자열 입력

```python
name = input("당신의 이름은?")
print(f"안녕하세요, {name}님!")
```

f-string 사용법   

## 3. 사칙연산
프로그래밍 언어는 기본적으로 연산을 위한 도구다.   

```python
print(1+2)  # 3
print(1-2)  # -1
print(1*2)  # 2
print(1/2)  # 0.5
print(2**2)  # 4
print(7%3)  # 1 (나머지를 반환)
print(7//4)  # 1 (몫을 반환)
```

## 4. 자료형이란?
숫자(정수/실수), 문자열, 리스트, 사전 등   

## 5. Python의 동적 타이핑
Python은 변수 초기화 시 타입을 자동으로 정해준다.   
### Python에서도 정적 타이핑이 가능하다.   
https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=passion053&logNo=221070020739

---

# 과제

1. 사용자의 이름을 입력받아 환영 인사해주기
2. 사용자의 생년을 입력받아 나이를 계산해주기
