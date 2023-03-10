---
title: "[C/C++] 자료구조를 공부하기 전 필요한 C 문법 총 정리! - 3"
categories: [C, Language, Data Structure]
tags: [문법, Language, C]
---
> 1. [Hello World!](https://zinovy124.github.io/c/language/data%20structure/the-C-language-1/)
> 2. [변수와 데이터 타입](#변수와-데이터-타입)
> 3. [조건문과 반복문]()
>> 1. [조건문]()
>> 2. [반복문]()
> 4. [함수]()
> 5. [배열]()
> 6. [포인터]()
> 7. [배열과 포인터]()
> 8. [메모리 공간과 데이터 공유]()
> 9. [메모리 동적 할당]()
> 10. [사용자 정의 자료형]()
---

# 조건문과 반복문

## 조건문(Condition)
다들 잘 아시다시피 if 혹은 switch 밖에 없습니다.   
<br>

### if Condition
```c
if (condition_1) {
    // Runs when condition_1 is true
} else if (condition_2) {
    // Runs when condition_2 is true
} else {
    // Runs when Condition_1 and Condition_2 weren't true
}
```
<br>

### switch Condition
```c
switch (caseNumber) {
    case 1:
        // Runs when caseNumber is 1
        break;
    case 2:
        // Runs when caseNumber is 2
        break;
    case 3:
        // Runs when caseNumber is 3
        break;

    default:
        // Runs when caseNumber ain't any of cases
}
```
switch문의 caseNumber는 정수 값입니다.   
<br>

## 반복문 (Iteration)
반복문은 for, while이 있고 do while은 사용하지 않습니다.

### for Iteration
```c
for (int i = 0; i < 10; i++) {
    // this block runs ten times
}
```
for의 조건 안에서 i가 선언이 안 된다면 아마 C99 이전의 Standard를 사용하고 있는 것일 수도 있습니다.   
예를 들어 C89 Standard까지만 해도...
```c
int i;
for (i = 0; i < 10; i++) {
    // ...
}
```
와 같이 코딩해야 했지요.   
C99부터는 가능합니다 ☺️   

### while Iteration
```c
while (condition) {
    // Runs while condition is true
}
```

---
조건문과 반복문입니다. 여기까지가 보통 기초라고 통칭하는 부분이죠.   
잘 숙지해두셔야 하겠습니다.