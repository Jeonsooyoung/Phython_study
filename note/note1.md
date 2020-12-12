# 1 THEORY (이론)
## 1. Data Type
- 변수 선언 :  <br>
              (number) a = 2, b = 3.12,    
              (text) c = "3",     
              (boolean) c = True,  d = False     
              (none) e = None (존재하지 않음)    
              
- 타입 표시 : print(type + (변수명) )
- variable type : 숫자, 문자, 참.거짓, null 값
- python 변수 컨벤 션 : snake case (ex) super_long_variable 


## 1.1 List in Python 
There is two sequence type  in python. one is list the other one is tuple.

하나의 변수에 여러개의 값을 넣고 싶을 때, 문자열로 저장할 경우, 데이터를 추가하거나, 각 데이터 값을 추출할 때 어려움.<br>
=> list 를 사용

- day = ["Mon", "Tue"] : 대괄호로 정의
- 파이썬 공식 문서에 리스트에 사용할 수 있는 연산자 있음.    
URL : https://docs.python.org/3/library/     
https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range    


## 1.2 Tuples and Dicts
1) Tuple
- days = ("Mon","Tue") 
- 아무도 변경 할 수 없는 리스트
- sequence를 변경 할 수 없음 
- list 와 같은 연산자 사용 가능 (50% 정도)
2) Dict 
-사전과 같이 key- value 로 이루어진 list 
person = {
  "name":"sooo",
  "age":15,
  "korean":True,
  "fav_food":["Cake","rice"]
}

print(person)
person["happy"] = True
print(person)

## 1.3 Built in Functions
function : 반복해서 사용할 수 있는 기능을 정의 
built in function : 파이썬에서 미리 정의된 함수. 언제나 사용 가능함(always available)
<br>
1) abs(x) : Return the <u>absolute value</u> of a number.<br>
The argument may be an integer, a floating point number(소수점 수), or an object implementing __abs__(). If the argument is a complex number(복소수?), its magnitude(크기) is returned.
<br><br>
2) all(iterable)<br>
* iterable 객체 - 반복 가능한 객체 <br>
* 대표적으로 iterable한 타입 - list, dict, set, str, bytes, tuple, range <br>
Return True if all elements of the iterable are true (or if the iterable is empty).
<br><br>
3) any(iterable)¶<br>
Return True if any element of the iterable is true. If the iterable is empty, return False.
<br><br>
4) ascii(object)



# 1.4 Creating a Your First Python Function     
define a function     
def 로 함수 정의     
def say_hello () :     
  print ("hello")    
  
- 파이썬은 중괄호로 함수의 시작과 끝을 판단하지 않음.    
indentation(들여쓰기로) function의 안을 표시함.(보통tab키로 들여씀)    
- 함수 명 뒤에 괄호를 추가하면 function을 실행함    


# 1.5 Function Arguments (positional arguments)
- print도 function 중 하나임. print function은 괄호 안에 뭔가 넣는 것을 허용한다.       
function 에 data의 input 된 data가 필요할 경우가 있기 때문       
함수를 정의할 때 function 이름을 정의하고, 괄호 안에 뭔가를 넣을 수 있도록 허용해야한다.    
그리고 function 이 가질 수 있는 arguments(인자)에 이름을 지어줄 수 있음.    

<code>
  def say_hello(who) : 
    print("hello", who)
</code>

- arguments에 기본값을 추가할 수 있음. 


# 1.6 Returns
-function의 결과물. 반환값을 의미    
return 하는 순간 해당 함수는 종료됨. 함수 내에서 return 은 한번만 실행됨. 

-예제에서 사용한 print함수는 결과를 단순 console에만 출력함    
이는 print로 함수를 호출할 경우, 해당 함수 안에 return  값이 아닌 print 함수가 있으면 
아무런 결과 출력 되지 않음 ex) 
def p_plus(a,b) : 
  print(a+b)
  
p_result = p_plus(2,3)
print(p_result)

# 1.7 Keyworded Arguments
- 인자인데, 위치가 아닌 arguments의 이름으로 쌍을 이루어줌    
인자의 순서를 신경 쓸 필요가 없고, 인자의 이름만 신경써주면 됨. 
- string 안에 변수를 포함시키고 싶으면 따옴표 가장 앞에 f(format)를 추가하고 변수의 이름에 중괄호 감싸주기     
문자열끼리 + 를 이용해서 연결할 수 있음. 


<code>
def p_plus(a=1,b=2) : 
  print(a+b)
</code>

# 1.8 Code Challenge (계산기)
- 7가지 function 만들기 
plus(+), minus(-), times(*), division(/), negation(//), power(**) ,reminder (%)<br>     
-숫자뿐 아니라 문자열 타입이 추가될 수도 있음 (오류체크)

# 1.9 Conditionals part One

# 1.10 if else and or

# 1.11 for in

# 1.12 Modules



