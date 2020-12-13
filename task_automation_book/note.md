# 목차 
[Part1. 프로그래밍 언어에 대한 이해](#1.프로그래밍-언어에-대한-이해)  
&nbsp;&nbsp;[1.파이썬이란](#1.-파이썬이란)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)프로그래밍이란](#1-프로그래밍이란)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)파이썬 특징](#2-파이썬특징)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)파이썬 설치하기](#3-파이썬-설치하기)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)파이썬 시작하기](#4-파이썬-시작하기)   
&nbsp;&nbsp;[2.변수와 자료형](#2.-변수와-자료형)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)변수와 자료형](#1-변수와-자료형)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)숫자 자료형](#2-숫자-자료형)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)문자열 자료형](#3-문자열-자료형)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)리스트 자료형](#4-리스트-자료형)   
&nbsp;&nbsp;&nbsp;&nbsp;[5)튜플 자료형](#5-튜플-자료형)   
&nbsp;&nbsp;&nbsp;&nbsp;[6)딕셔너리 자료형](#6-딕셔너리-자료형)   

&nbsp;&nbsp;[3.제어문](#3.-제어문)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)조건문,if문](#1-조건문,if문)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)반복문,for문](#2-반복문,for문)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)반복문,while문](#3-반복문,while문)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)반복문에서 사용하는 구문:break,continue](#4-반복문에서-사용하는-구문:break,continue)   

&nbsp;&nbsp;[4.함수와 클래스](#4.-함수와-클래스)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)함수란?](#1-함수란?)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)반환함수,return](#2-반환함수,return)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)내장 함수](#3-내장-함수)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)클래스란](#4-클래스란)   
&nbsp;&nbsp;&nbsp;&nbsp;[5)클래스활용](#5-클래스활용)   
&nbsp;&nbsp;&nbsp;&nbsp;[6)그외문법](#6-그외문법)   

[Part2. 업무 자동화로 일 편하게 하기](#2.업무-자동화로-일-편하게-하기)   
&nbsp;&nbsp;[1.파일다루기](#1.-파일다루기)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)라이브러리소개](#1-라이브러리소개)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)도전업무1,스캔파일폴더정리](#2-도전업무1,스캔파일폴더정리)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)자동화](#3-자동화)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)라이브러리](#4-라이브러리)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)도전업무2,csv파일읽기](#2-도전업무2,csv파일읽기)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)자동화로해결](#3-자동화로해결)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)기타파일함수](#4-기타파일함수) 

&nbsp;&nbsp;[2.엑셀다루기](#2.-엑셀다루기)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)라이브러리소개](#1-라이브러리소개)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)도전업무,엑셀파일취합](#2-도전업무,엑셀파일취합)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)자동화](#3-자동화)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)라이브러리](#4-라이브러리)    

&nbsp;&nbsp;[3.이메일다루기](#3.-이메일다루기)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)라이브러리소개](#1-라이브러리소개)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)이메일발송원리](#2-이메일발송원리)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)도전업무,메일보내기](#3-도전업무,메일보내기)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)자동화](#4-자동화)   
&nbsp;&nbsp;&nbsp;&nbsp;[5)심화:다수에게발송](#5-심화:다수에게발송)    

&nbsp;&nbsp;[4.기사수집하기](#4.-기사수집하기)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)RSS](#1-RSS)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)라이브러리소개](#1-라이브러리소개)    
&nbsp;&nbsp;&nbsp;&nbsp;[3)도전업무,포털기사수집](#3-도전업무,포털기사수집)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)자동화](#4-자동화)     

&nbsp;&nbsp;[5.웹사이트기초](#5.-웹사이트기초)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)웹사이트분석](#1-웹사이트분석)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)라이브러리소개](#2-라이브러리소개)    
&nbsp;&nbsp;&nbsp;&nbsp;[3)웹사이트,뉴스일부제목가져오기](#3-웹사이트,뉴스일부제목가져오기)    
&nbsp;&nbsp;&nbsp;&nbsp;[4)도전업무,포털기사수집](#4-도전업무,포털기사수집)   
&nbsp;&nbsp;&nbsp;&nbsp;[5)자동화](#5-자동화)     

&nbsp;&nbsp;[6.웹사이트심화](#6.-웹사이트심화)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)인스타태그검색좋아요누르기](#1-인스타태그검색좋아요누르기)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)중고나라검색결과가져오기](#2-중고나라검색결과가져오기)    
&nbsp;&nbsp;&nbsp;&nbsp;[3)11번가검색결과정리하기](#3-11번가검색결과정리하기)      
&nbsp;&nbsp;&nbsp;&nbsp;[4)라이브러리살펴보기](#4-라이브러리살펴보기)     

[Part3. 컴퓨터가 스스로 일하게 하기](#3.컴퓨터가-스스로-일하게-하기)     
&nbsp;&nbsp;[1.프로그램스케쥴링](#1.-프로그램스케쥴링)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)cron](#1-cron)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)cron설치](#2-cron설치)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)cron설정](#3-cron설정)   
&nbsp;&nbsp;&nbsp;&nbsp;[4)cron실습](#4-cron실습)    

&nbsp;&nbsp;[2.cron모니터링](#2.-cron모니터링)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)11번가모니터링](#1-11번가모니터링)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)키워드과제공고](#2-키워드과제공고)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)라이브러리살펴보기](#3-라이브러리살펴보기)    

[Part4. 파이썬 좀더 알아보기](#4.파이썬-좀-더-알아보기)    
&nbsp;&nbsp;[1.디버깅](#1.-디버깅)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)오류메시지해석](#1-오류메시지해석)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)오류해결](#2-오류해결)   

&nbsp;&nbsp;[2.IDE사용법,PyCharm](#2.-IDE사용법,PyCharm)   
&nbsp;&nbsp;&nbsp;&nbsp;[1)PyCharm설치](#1-PyCharm설치)   
&nbsp;&nbsp;&nbsp;&nbsp;[2)프로젝트생성](#2-프로젝트생성)   
&nbsp;&nbsp;&nbsp;&nbsp;[3)파이썬파일실행](#3-파이썬파일실행)     
&nbsp;&nbsp;&nbsp;&nbsp;[4)디버깅](#4-디버깅)    


## 1.프로그래밍 언어에 대한 이해
## 2.업무 자동화로 일 편하게 하기
## 3.컴퓨터가 스스로 일하게 하기
## 4.파이썬 좀 더 알아보기




