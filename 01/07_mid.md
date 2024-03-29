## 1차 중간점검 
### 출력

- 아래 문장을 출력하세요.
  - 작은 따옴표도 출력합니다.

```python
'python'은 프로그래밍 언어입니다.
```
```python
print(_______________________)
```


### 숫자형

- 화씨온도(℉)를 섭씨온도(℃)로, 섭씨온도(℃)를 화씨온도(℉)로 바꾸려고 합니다. 두 온도 사이의 환산 공식은 다음과 같습니다.       
  - 화씨온도(℉)에서 섭씨온도(℃)로 환산 : (화씨온도 - 32) ÷ 1.8 = 섭씨온도
  - 섭씨온도(℃)에서 화씨온도(℉)로 환산 : (섭씨온도 x 1.8) + 32 = 화씨온도

```python
 # 화씨 온도입니다. 섭씨 온도는 0도 입니다.
temperature1 = 32

# 섭씨 온도입니다. 화씨 온도는 89.6도 입니다.
temperature2 = 32

convert1 = @@@
convert2 = @@@

print('화씨 {}도는 섭씨 {}도'.format(temperature1, convert1)) # 화씨 32도는 섭씨 0도
print('섭씨 {}도는 화씨 {}도'.format(temperature2, convert2)) # 섭씨 32도는 화씨 89.6도
```

### 변수
- 'year'이라는 이름을 가진 변수를 선언하고 올해의 년도를 할당하세요.

```python
# 변수명 = 값
```

### 문자열
- 다음 중 실행이 불가능한 코드는 몇번째 줄에 있나요?
  - 하나 이상일 수 있습니다.

```
print('Hello world!')
print("Hello world!")
print(''Hello world!'')
print(""Hello world!"")
print('''Hello world!''')
print("""Hello world!""")
```

- 두 변수를 사용하여 아래 문장을 출력하세요.
  - hello world hello world hello world hello world hello world
  - s1 = "hello"
  - s2 = "world"
```python
s1 = 'hello'
s2 = 'world'
print(@@@)
```

- 코드의 실행 결과를 옆에 주석(comment - #)으로 적어보세요.
  - 무엇이 다른가요?

```python
a = 2023
b = 12
print(a + b)

a = "2023"
b = "12"
print(a + b)
```

- 아래 문자열을 변수에 저장하고 다양한 문자를 출력해보세요.
  - Love yourself.
  - L, v, u, s, f
  
```python
s = 'Love yourself.'
print(s[0]) # L
print(@@@) # v
...
```


- 아래 코드를 실행하면 어떻게 동작할지 예상해보고 결괏값을 적어보세요.

```python
sentence = "Python에서 숫자 10과 문자 '10'은 다르다."

print(sentence[5])
print(sentence[-5])
print(sentence[10:12])
print(sentence[13:])
```


- 아래 문장은 어떤 게임에서 몬스터가 데미지를 받을 때 나오는 문장입니다. 받은 데미지를 다양하게 출력해보세요.
  - 데미지 10, 50, 297 출력

```python
# s.format(____) 혹은 f'____' 사용
s = '공격받은 몬스터는 {}의 데미지를 받았습니다.'
print(@@@)
print(@@@)
print(@@@)
```


- 아래 코드에서 오류가 발생하는 이유를 코드 옆에 주석(comment)으로 작성하세요.

```python
age = 12
age[0]

age = '12'
age[0]
```


### 입/출력

- '당신의 나이는?' 문자열을 출력하고, 사용자의 입력을 받아서 태어난 연도를 출력하세요.
  - input 함수와 형변환 함수(int)를 사용합니다.
```python
age = @@@ 
year = @@@@ - age
print('당신의 올해 나이는 {}살 입니다. 당신은 {}년에 태어났습니다.'.format(age, year))
```

- "20240101Sunny" 형태의 문자열을 입력받아 '년/월/일/날씨' 로 구분하여 출력하세요.

```python
s = @@@
year = s[@@:@@]
month = s[@@:@@]
day = s[@@:@@]
weather = s[@@:@@]
print("{}년 {}월 {}일 / 날씨 : {}".@@@)
```

### 함수

- 파라미터로 넘어온 문자열 끝에 ":D" 문자열을 붙여 출력하는 'smile' 함수를 정의하세요.
  - 문자열 더하기(+)를 사용합니다.
  - '안녕하세요' + ' :D' => '안녕하세요 :D'

```python
# 함수 정의
_____ smile(s):
    end = ' :D'
    print(@@@)

# 함수 호출
smile('안녕하세요') # '안녕하세요 :D' 출력
smile('날씨가 좋아요') # '날씨가 좋아요 :D' 출력
```

- 파라미터로 넘어온 문자열 끝에 ":(" 문자열을 붙여 리턴하는 'upset' 함수를 정의하세요.
  - 문자열 더하기(+)를 사용합니다.
  - '넘어졌어요' + ' :(' => '넘어졌어요 :('

```python
# 함수 정의
_____ upset(s):
    end = ' :('
    return @@@

# 함수 호출
s1 = upset('넘어졌어요')
print(s1) # '넘어졌어요 :(' 출력
s2 = upset('오늘은 조금 피곤해요')
print(s2) # '오늘은 조금 피곤해요 :(' 출력
```


- 원화를 넣으면 달러로 대략 얼마인지 계산하여 리턴해주는 'exchange' 함수를 정의하세요.
  - 1달러는 원화로 약 1300원 입니다. 
  - 2000원, 13000원, 1000000원을 넣어 함수를 호출하세요.

```python
# 함수 정의
def @@@(won) :
    @@@
    return dollar

# 함수 호출
print('${}'.format(exchange(1300))) # $1
print('${}'.format(exchange(2600))) # $2
print('${}'.format(exchange(13000))) # $10
print('${}'.format(exchange(1000000))) # $769.23

won = int(input('환전할 원화 : '))
dollar = exchange(won)
print('당신은 ${} 를 환전했습니다.'.format(dollar))
```


### bool 자료형


- 다음 중 불 자료형을 모두 고르세요.
  - 불(bool) 자료형이란 참(True)과 거짓(False)을 나타내는 자료형입니다. 

```
a = True
b = False
c = true
d = false
e = TRUE
f = FALSE
```


### 비교/논리 연산자

- 아래 코드를 실행하면 어떤 결과가 나올지 적어보세요.

```python
x = 4 
y = 9
print(x > y)
print(x < y)
print(x == y)
print(x != y)
print(x >= y)
print(x <= y)
print(x/10 < y)

print(10 == 10 and 10 != 5)
print(4 > 2 and 7 == 3)
print(10 < 5 or 10 > 3)
print(9 < 7 or 7 < 3)
print(not 10 >= 5)
print(not 10 <= 10)
```

### 조건문


- 아래 코드를 실행하면 어떤 결과가 나올지 적어보세요.

```python
print("1")
if True:
    print("2")
else :
    print("3")
print("4")
```

```python
print("1")
if 3 > 7:
    if 10 == 9:
        print("2")
    else:
        print("3")
else :
    print("4")
print("5")
```

```python
print("1")
if 'coding' == 'coding':
    if 'whale' == 'Whale':
        print("2")
    elif 3 != 3:
        print("3")
    else:
        print("4")
elif 3 == 3:
    print("5")
else :
    print("6")
print("7")
```


- 사용자로부터 하나의 숫자를 입력 받아 짝수/홀수를 출력하는 함수를 작성하세요.
  - 짝수/홀수인지 판별할때는 '%' 기호를 주로 사용합니다.
  - 짝수는 2로 나눈 나머지가 0, 홀수는 2로 나눈 나머지가 1입니다.

```python
def even_odd(number):
    if @@@:
        print("짝수")
    else:
        print("홀수")

number = input("숫자 입력 : ")
even_odd(int(number))
```



- 사용자로부터 세 개의 숫자를 입력받은 후 가장 작은 숫자를 출력하세요.

```python
num1 = input("input number1: ")
num2 = input("input number2: ")
num3 = input("input number3: ")
# 코드 작성
if @@@:
    print('{}이 가장 작은 숫자입니다.'.format(num1))
elif @@@:
    print('{}이 가장 작은 숫자입니다.'.format(num2))
elif @@@:
    print('{}이 가장 작은 숫자입니다.'.format(num3))
else:
    print(@@@) # 적절한 문자열을 출력하세요.
```


- 부산으로 가는 교통편이 'Bus', 'Ship', 'Airplane' 총 3가지일때 타고갈 교통편을 입력받아, 성인 요금과 어린이 요금을 출력하세요.   
  - 성인 요금
    - Bus : 50000원 
    - Ship : 70000원
    - Airplane : 100000원
  - 어린이 요금은 성인 요금에서 50% 할인됩니다.

```python
def print_price(transportation):
    adult_price = 0
    child_price = 0
    
    @@@
    
    print('{}의 성인 요금은 {}원, 어린이 요금은 {}원 입니다.'.format(transportation, adult_price, child_price))


transportation = input("사용할 교통편 : ")
print_price(transportation)
```

### 반복문

- 1부터 100 사이의 숫자 중 7의 배수를 모두 출력하세요.
  - for 문과 while 문을 사용하여 두 방법으로 각각 코딩하세요.

```python
for i in range(@@@, @@@, @@@):
    if @@@:
        print(@@@)
        

i = 0
while @@@:
    i = i + 1
    if @@@:
        print(@@@)
```

- 한국의 수도를 묻고 답변을 받아 정답인지 알려주는 프로그램을 작성하세요.
  - 입력은 계속 받을 수 있으며 '그만' 을 입력시 프로그램이 종료됩니다.

```python
while True:
    capital = input('한국의 수도는? : ')
    
    if capital == '그만' : 
        @@@
    elif @@@:
    ...

```

- 점수 구간에 해당하는 등급이 아래와 같이 정의되어 있습니다. 사용자로부터 score를 입력받아 등급을 출력하세요.
  - 입력은 계속 받을 수 있으며 '-1' 을 입력시 프로그램이 종료됩니다.


```python
# 80~100 : A등급
# 60~79 : B등급
# 40~59 : C등급
# 20~39 : D등급
# 0~19 : E등급
# 100 초과, 0 미만 : 잘못된 입력

while True:
    score = input("점수: ")
    
    @@@
```


- 사용자에게 나이를 입력받아 나이대 구간에 따라서 결과를 출력하세요.
  - 입력은 계속 받을 수 있으며 '-1' 을 입력시 프로그램이 종료됩니다.
  - 초등학생 나이는 8살 이상 13살 이하입니다.
  - 중학생 나이는 14살 이상 16살 이하입니다.
  - 고등학생 나이는 17살 이상 19살 이하입니다.
  - 미취학 아동은 8살 미만, 성인은 20살 이상입니다. 

```python
age = int(input('나이 : ')) # 사용
```


### 자료형
- 아래 변수들의 데이터 타입이 무엇인가요?
  - 유효하지 않은 데이터 타입인 경우 error 가 발생합니다.
  
```python
a = 1000
b = '1000'
c = True
d = 'False'
e = 'hello world!'
f = TRUE
g = 30.1
h = '2023'
i = true
j = 'false'
k = -59
l = 0
m = '0'
n = '2023'+'11'
o = False
p = 1000 + 100 - 99
q = '*' * 10
r = 10 * 10
s = '100' <= 10
t = 100 > 10
u = false
```

### 반복문2
- 사용자의 입력을 받아 그 수만큼 직사각형 별(*)을 출력하는 프로그램을 작성하세요.

```python
number = input('숫자 입력 : )
@@@

# 3 입력
***
***
***

# 5 입력
*****
*****
*****
*****
*****
```

- 사용자의 입력을 받아 그 수만큼 직각 삼각형 별(*)을 출력하는 프로그램을 작성하세요.

```python
number = input('숫자 입력 : )
@@@

# 3 입력
*
**
***

# 5 입력
*
**
***
****
*****
```

- 사용자의 입력을 받아 그 수만큼 직각 삼각형 별(*)을 출력하는 프로그램을 작성하세요.

```python
number = input('숫자 입력 : )
@@@

# 3 입력
  *
 **
***

# 5 입력
    *
   **
  ***
 ****
*****
```

- 사용자의 입력을 받아 그 수만큼 삼각형 별(*)을 출력하는 프로그램을 작성하세요.

```python
number = input('숫자 입력 : )
@@@

# 3 입력
  *
 ***
*****

# 5 입력
    *
   ***
  *****
 *******
*********
```

- 두 개의 숫자를 입력받아 합/차/곱/나눗셈을 출력하는 'operations' 함수를 정의하세요.
  - 두 숫자는 input 함수를 사용하여 입력합니다.
  - 각각의 결과에서 `+, -, *, /` 연산자를 사용합니다.
  - 합/차/곱/나눗셈 값을 모두 더한 결과를 return 합니다.

```python
# 함수 정의
def operations(@@@, @@@):
    r1 = num1 + num2
    r2 = @@@
    r3 = @@@
    r4 = @@@
    print('{} + {} = {}'.format(@@@, @@@, @@@))
    print('{} - {} = {}'.format(@@@, @@@, @@@))
    print('{} * {} = {}'.format(@@@, @@@, @@@))
    print('{} / {} = {}'.format(@@@, @@@, @@@))
    return @@@

# 함수 호출
num1 = @@@
num2 = @@@
result = operations(@@@, @@@)
print(result)
```
