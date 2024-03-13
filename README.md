# Python-20240313
- 1.Python Syntax
    
    Python Syntax
    
    공백이 없으면 오류가 발생한다.
    
    일반적으로 4개의 공백이 사용된다.
    
    적어도 하나는 필수이다.
    
    ```jsx
    if 5 > 2:
      print("Five is greater than two!")
    ```
    
    변수에 값 할당 →>>변수 생성
    
    ```jsx
    x = 5
    y = "Hello, World!"
    
    ```
    
    #은 주석(글의 뜻을 해석)
    
    ```jsx
    #This is a comment.
    ```
    
- 2.Python Comments
    
    Python은 주석 뒤 무시
    
    ```jsx
    #This is a comment
    print("Hello, World!")
    
    ```
    
- 3.Python Variables
    
    다른 유형으로 변수 설정 가능
    
    ```jsx
    x = 5
    y = "John"
    print(x)
    print(y)
    
    ```
    
    변수는 더욱 더 길게 설정할 수 있다.
    
    ```jsx
    myvar = "John"
    my_var = "John"
    _my_var = "John"
    myVar = "John"
    MYVAR = "John"
    myvar2 = "John"
    
    ```
    
    여러 값으로 설정 가능
    
    ```jsx
    x, y, z = "Orange", "Banana", "Cherry"
    print(x)
    print(y)
    print(z)
    
    ```
    
    +쉼표로 연산 가능(수와 문자는 연산 X)
    
    ```jsx
    x = "Python"
    y = "is"
    z = "awesome"
    print(x, y, z)
    
    ```
    
- 4.Python Data Types
    
    ```jsx
    문자열 유형: str
    숫자(정수,실수) 유형: int, float, complex
    시퀀스 유형: list, tuple, range
    매핑 유형: dict
    세트 유형: set,frozenset
    부울 유형: bool
    바이너리 유형: bytes, bytearray, memoryview
    없음 유형: NoneType
    
    ```
    
    type()→데이터 유형 추출
    
    ```jsx
    x = 5
    print(type(x))
    
    ```
    
- 5.Python Numbers
    
    Python의 세가지 유형
    
    ```jsx
    int 정수
    float 실수
    complex 복소수
    
    x = 1    # int
    y = 2.8  # float
    z = 1j   # complex
    ```
    
- 6.Python Casting
    
    변수 유형 지정
    
    ```jsx
    정수
    x = int(1)   # x will be 1
    y = int(2.8) # y will be 2
    z = int("3") # z will be 3
    
    실수
    x = float(1)     # x will be 1.0
    y = float(2.8)   # y will be 2.8
    z = float("3")   # z will be 3.0
    w = float("4.2") # w will be 4.2
    
    문자열
    x = str("s1") # x will be 's1'
    y = str(2)    # y will be '2'
    z = str(3.0)  # z will be '3.0'
    
    ```
    
- 7.Python Strings
    
    ‘나’로 표현
    
    ```jsx
    print("Hello")
    print('Hello')
    
    ```
    
    슬라이스 구문 사용→문자로 변환
    
    ```jsx
    b = "Hello, World!"
    print(b[2:5])
    
    b = "Hello, World!" #처음부터
    print(b[:5])
    
    ```
    
    변환
    
    ```jsx
    a = "Hello, World!" #소문자로
    print(a.lower())
    
    a = " Hello, World! " #공백 제거
    print(a.strip()) # returns "Hello, World!"
    
    a = "Hello, World!" #문자열 바꾸기
    print(a.replace("H", "J"))
    
    a = "Hello, World!" #문자열 분할
    print(a.split(",")) # returns ['Hello', ' World!']
    
    ```
    
    연결
    
    ```jsx
    a = "Hello"
    b = "World"
    c = a + b
    print(c)
    
    a = "Hello" #공백 추가
    b = "World"
    c = a + " " + b
    print(c)
    ```
    
    형식 지정
    
    ```jsx
    age = 36
    txt = "My name is John, and I am {}"
    print(txt.format(age))
    
    quantity = 3
    itemno = 567
    price = 49.95
    myorder = "I want {} pieces of item {} for {} dollars."
    print(myorder.format(quantity, itemno, price))
    
    quantity = 3
    itemno = 567
    price = 49.95
    myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
    print(myorder.format(quantity, itemno, price))
    ```
    
    이스케이프(escape) 문자
    
    ```jsx
    txt = "We are the so-called \\"Vikings\\" from the north."
    ```
    
- 8.Python Booleans
    
    True 또는 False 출력
    
    ```jsx
    print(10 > 9)
    print(10 == 9)
    print(10 < 9)
    
    a = 200
    b = 33
    if b > a:
      print("b is greater than a")
    else:
      print("b is not greater than a")
    
    print(bool("Hello"))
    print(bool(15))
    
    x = "Hello"
    y = 15
    print(bool(x))
    print(bool(y)
    ```
    
- 9.Python Operators
    
    연산시에는 +를 사용한다
    
    ```jsx
    print(10 + 5)
    
    ```
    
- 10.Python Lists
    
    목록은 단일 변수에 여러 항목을 저장할 수 있다.
    
    변경이 가능하다.
    
    중복이 허용된다.
    
    목록 길이→len()
    
    목록 항목은 모든 데이터 유형이 가능하다
    
    type()
    
    list()
    
    ```jsx
    thislist = ["apple", "banana", "cherry"]
    print(thislist)
    
    thislist = ["apple", "banana", "cherry", "apple", "cherry"]
    print(thislist)
    
    thislist = ["apple", "banana", "cherry"]
    print(len(thislist))
    
    list1 = ["apple", "banana", "cherry"]
    list2 = [1, 5, 7, 9, 3]
    list3 = [True, False, False]
    
    list1 = ["abc", 34, True, 40, "male"]
    
    mylist = ["apple", "banana", "cherry"]
    print(type(mylist))
    
    thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
    print(thislist)
    
    ```
    
- 11.Python…Else
    
    if문 종류
    
    ```jsx
    Equals: a == b
    Not Equals: a != b
    Less than: a < b
    Less than or equal to: a <= b
    Greater than: a > b
    Greater than or equal to: a >= b
    
    ```
    
- 12.Python While Loops
    
    두가지 기본 루프 명령
    
    ```jsx
    while 루프
    for 루프
    
    ```
    
    while 루프
    
    break 루프
    
    게속 진술
    
    else 문
    
    ```jsx
    i = 1
    while i < 6:
      print(i)
      i += 1
    
    i = 1
    while i < 6:
      print(i)
      if i == 3:
        break
      i += 1
    
    i = 0
    while i < 6:
      i += 1
      if i == 3:
        continue
      print(i)
    
    i = 1
    while i < 6:
      print(i)
      i += 1
    else:
      print("i is no longer less than 6")
    
    ```
    
- 13.Python For Loops
    
    for 루프→시퀀스(목록,튜플,사전,집합,또는 문자열)반복
    
    ```jsx
    fruits = ["apple", "banana", "cherry"]
    for x in fruits:
      print(x)
    
    ```
    
    문자열을 통한 반복
    
    ```jsx
    for x in "banana":
      print(x)
    ```
    
    break 문
    
    ```jsx
    fruits = ["apple", "banana", "cherry"]
    for x in fruits:
      print(x)
      if x == "banana":
        break
    
    fruits = ["apple", "banana", "cherry"]
    for x in fruits:
      if x == "banana":
        break
      print(x)
    
    ```
    
    계속 진술
    
    ```jsx
    fruits = ["apple", "banana", "cherry"]
    for x in fruits:
      if x == "banana":
        continue
      print(x)
    
    ```
    
    range() 함수
    
    ```jsx
    for x in range(6):
      print(x)
    
    for x in range(2, 6):
      print(x)
    
    for x in range(2, 30, 3):
      print(x)
    ```
    
    for 루프 else
    
    ```jsx
    for x in range(6):
      print(x)
    else:
      print("Finally finished!")
    
    for x in range(6):
      if x == 3: break
      print(x)
    else:
      print("Finally finished!")
    
    ```
    
    중첩 루프
    
    ```jsx
    adj = ["red", "big", "tasty"]
    fruits = ["apple", "banana", "cherry"]
    
    for x in adj:
      for y in fruits:
        print(x, y)
    
    ```
    
    패스 설명
    
    ```jsx
    for x in [0, 1, 2]:
      pass
    
    ```
