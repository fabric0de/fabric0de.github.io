---
title: JS 데이터 타입
date: 2023-11-17 21:14:00 +0800
categories: [프론트엔드, JavaScript]
tags: [JS, DataType, JavaScript, String, Number]
---


# JavaScript 데이터타입

데이터 타입은 프로그래밍 언어에서 사용할 수 있는 데이터의 종류를 말합니다.  
JavaScript의 데이터 타입은 크게 원시 타입(Primitive Types)과 객체 타입(Object Types)으로 나누어 집니다. 


## 원시 타입 (Primitive Types)

### String
텍스트 데이터를 나타내며 큰따옴표, 작은따옴표, 또는 백틱으로 묶어 표현합니다.
```javascript
let name = "Hyeon"; // 큰따옴표 사용
let greeting = 'Hello'; // 작은따옴표 사용
let sentence = `My name is ${name}`; // 백틱과 템플릿 리터럴 사용
```

### Number
정수 및 부동 소수점 숫자를 나타냅니다.
```javascript
let integer = 10;
let float = 10.5;
```

### BigInt
매우 큰 정수를 나타낼 때 사용되고 숫자 끝에 `n`을 붙여 표현합니다.
```javascript
let bigInteger = 1234567890123456789012345678901234567890n;
```

### Boolean
논리적 값인 `true`와 `false`를 나타냅니다.
```javascript
let isTrue = true;
let isFalse = false;
```

### Undefined
변수가 값 없이 선언되었을 때 자동으로 할당되는 값입니다.
```javascript
let notAssigned;
console.log(notAssigned); // undefined
```

### Null
"값이 없음"을 의도적으로 나타내는데 사용되고 명시적으로 할당합니다.
```javascript
let empty = null;
```

### Symbol
고유하고 변경 불가능한 값으로 주로 객체 속성의 키로 사용됩니다.  
Symbol은 ES6 버전부터 새롭게 추가 되었습니다.
```javascript
let symbol1 = Symbol("id");
let symbol2 = Symbol("id");
console.log(symbol1 === symbol2); // false 각 Symbol은 고유합니다.
```


## 객체 타입 (Object Types)

### Object
키와 값의 집합으로, 데이터 구조를 나타내는 데 사용됩니다.   
객체는 `{}`를 사용하여 생성할 수 있으며, 다양한 데이터 타입을 값으로 가질 수 있습니다.
```javascript
let person = {
  name: "John",
  age: 30,
  isEmployed: true
};
```

### Array
순서가 있는 데이터 집합을 나타냅니다.   
배열은 `[]`를 사용하여 생성합니다.  
```javascript
let numbers = [1, 2, 3, 4, 5];
```

### Function
실행 가능한 코드 블록을 나타내며, `function` 키워드를 사용하여 정의됩니다.
```javascript
function greet(name) {
  return `Hello, ${name}!`;
}
```
  
  
# 참고 자료
- <a href="https://developer.mozilla.org/ko/docs/Web/JavaScript/Data_structures" target="_blank">JavaScript의 타입과 자료구조 - MDN</a>