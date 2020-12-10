# 1 THEORY
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



