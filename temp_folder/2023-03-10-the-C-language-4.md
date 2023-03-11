---
title: "[C/C++] 자료구조를 공부하기 전 필요한 C 문법 총 정리! - 4"
categories: [C, Language, Data Structure]
tags: [문법, Language, C]
---
> 1. [Hello World!](https://zinovy124.github.io/c/language/data%20structure/the-C-language-1/)
> 2. [변수와 데이터 타입](#변수와-데이터-타입)
> 3. [조건문과 반복문]()
> 4. [함수]()
> 5. [배열]()
> 6. [포인터]()
> 7. [배열과 포인터]()
> 8. [메모리 공간과 데이터 공유]()
> 9. [메모리 동적 할당]()
> 10. [사용자 정의 자료형]()
---
함수로 시작해서 함수로 끝나는 C언어, 함수 지향 프로그래밍의 꽃이죠, 함수에 대해서 알아보겠습니다. (사실 C의 꽃은 포인터입니다.)

# 함수 선언
```c
void someFunc(void) {
    printf("Hello World!");
}
```
와 같이 함수를 선언할 수 있습니다. 이 함수가 사용될 곳보다 상단부에 선언되어야 합니다.
여기서,
![Function-image-1](https://github.com/zinovy124/zinovy124.github.io/blob/main/_posts/images/%EB%B8%94%EB%A1%9C%EA%B7%B8%20%EC%9E%90%EB%A3%8C-2.jpg?raw=true)

1번이 함수가 리턴하는 값의 타입을 명시하는 곳이고 2번은 파라미터 자리이다.
`int parm`과 같이 명시하면 된다.

# 함수 사용
```c
someFunc();
```
그냥 중괄호 붙여서 사용하면 됩니다.

# 함수 프로토타입
함수를 먼저 사용하겠다고 명시만 해주고 뒤쪽에 선언할 수도 있다.

모든 코드를 작성해보겠다.

```c
#include <stdio.h>

void someFunc(void);

int main(void) {
    someFunc();

    return 0;
}

void someFunc(void) {
    printf("Hello World!");
}
```

와 같이 작성했을 때, 3 line의 `void someFunc(void);`를 프로토타입이라고 부른다.

---
이따금 다시 환기해드리지만 자료구조를 배우기 전 간단한 C Remind입니다.
본격적으로 C를 다루는 코너는 이따금 편성해드리겠습니다.