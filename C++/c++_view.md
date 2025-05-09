## 📌 C++이란?

C++는 1980년대 초반 Bjarne Stroustrup이 개발한 **범용 프로그래밍 언어**

- **C 언어 기반**: C의 성능과 저수준 제어 기능을 그대로 계승
- **객체지향 프로그래밍(OOP)** 지원: 클래스, 상속, 다형성 등
- **절차적/객체지향/템플릿/제네릭 프로그래밍** 등 다양한 패러다임 지원
- **고성능**과 **시스템 수준 제어**가 필요한 소프트웨어 개발에 적합

> 대표 사용 분야: 운영체제, 게임 엔진, 임베디드 시스템, 로봇 소프트웨어 등

---

## 📌 객체지향 프로그래밍(Object-Oriented Programming, OOP)이란??

- 객체 지향 프로그래밍은 컴퓨터 프로그래밍 패러다임 중 하나로, 
프로그래밍에서 필요한 데이터를 추상화시켜 상태와 행위를 가진 객체를 만들고 그 객체들 간의 유기적인 상호작용을 통해 로직을 구성하는 프로그래밍 방법
- 각 객체는 속성(데이터)과 행동(기능)을 포함하며, 서로 상호작용을 통해 프로그램 작동

## 📌 객체란? 
- 객체는 클래스라는 설계도로부터 생성된, 메모리상에 존재하는 구체적인 데이터 단위

## 🧩 객체지향의 4대 핵심 개념

| 개념 | 설명 | 키워드 |
|------|------|--------|
| 캡슐화(Encapsulation) | 데이터와 메서드를 하나의 단위로 묶고 외부에서 직접 접근하지 못하도록 보호 | `private`, `public` |
| 상속(Inheritance) | 기존 클래스의 특성을 새로운 클래스가 물려받음 | `class Sub : public Super` |
| 다형성(Polymorphism) | 하나의 인터페이스로 다양한 기능 수행 | 오버로딩, 오버라이딩 |
| 추상화(Abstraction) | 불필요한 내부 구현은 숨기고 중요한 부분만 공개 | 인터페이스, 추상 클래스 |

## 🧩 객체지향을 사용하는 이유

- 현실 세계처럼 모델링이 직관적
- 코드 재사용이 쉬움 (상속)
- 유지보수가 편리함 (모듈화)
- 확장성이 높음 (다형성)


## ⚙️ C++ 빌드 과정

|단계|정의|하는 일|
|-----|-------|-------|
|전처리 (Preprocessing)|	컴파일 전에 #으로 시작하는 전처리 지시문을 처리하는 단계|	#include, #define, 조건부 컴파일, 주석 제거 등을 수행|
|컴파일 (Compilation)|	C++ 코드를 어셈블리어로 바꾸는 단계|	문법 체크, 타입 검사 후 사람이 쓴 코드를 기계가 이해하기 쉬운 **중간 코드(.s)**로 변환|
|어셈블 (Assembly)|	어셈블리어를 **기계어로 된 목적 코드(.o)**로 바꾸는 단계|	어셈블리 코드를 바이너리 목적 파일로 변환|
|링킹 (Linking)|	여러 개의 목적 파일과 라이브러리를 연결하여 **실행파일(.exe)**을 만드는 단계|	함수, 변수 등의 참조를 실제 주소로 연결하여 최종 실행 파일 생성|

## 📦 전체 요약: C++ 빌드 프로세스

```text

[소스코드.cpp]
     ↓ 전처리
[전처리된 코드]
     ↓ 컴파일
[어셈블리 코드 .s]
     ↓ 어셈블
[목적 코드 .o]
     ↓ 링커
[실행 파일 .exe]

---
