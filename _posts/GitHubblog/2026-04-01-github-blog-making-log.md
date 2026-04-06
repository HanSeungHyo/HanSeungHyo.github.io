---
title: "피보나치 수열을 해보자"
date: 2026-04-01
categories: [GitHubblog]
tags: [github-pages, jekyll, blog]
slug: github-blog-second
---

정처기를 풀다가 코드가 나와서 까먹기전에 풀이 과정을 적어보려고 한다

```c
#include <stdio.h>

int main() {
    int a[10]; //총 10개를 저장 (a[0] ~ a[9])
    a[0] = 0;
    a[1] = 1;//10개 중에 2개는 지정된상태

    for (int i = 0; i < 8; i++) { //채워진 a[1]부터 시작 a[2] ~ a[9]까지 채움 (총 8개)
        a[i + 2] = a[i + 1] + a[i]; //바로 앞 두 값을 더해서 다음 값을 만드는 피보나치 수열 규칙
    }

    printf("%d", a[9]); //%d 정수(int)를 출력할 때 쓰는 형식 지정자
}
```

피보나치 수열임을 알 수 있는 것은
a[i+2] = a[i+1] + a[i] → 피보나치 규칙
a[0]=0, a[1]=1 → 피보나치 시작값 이


챗지피티와 풀었던 문제
```c1
int a[10];
a[0] = 1;
a[1] = 1;

for (int i = 0; i < 8; i++) {
    a[i + 2] = a[i + 1] + a[i];
}
```

```c2
int a[10];
a[0] = 0;
a[1] = 1;

for (int i = 0; i < 8; i++) {
    a[i + 2] = a[i + 1] - a[i];
}
```

```c
int a[10];
a[0] = 0;
a[1] = 1;

for (int i = 2; i < 10; i++) {
    a[i] = a[i - 1] + a[i - 2];
}
```

```c
int a[10];
a[0] = 2;
a[1] = 3;

for (int i = 0; i < 8; i++) {
    a[i + 2] = a[i + 1] + a[i];
}
```

```c
int a[10];
a[0] = 0;

for (int i = 1; i < 10; i++) {
    a[i] = a[i - 1] + i;
}
```

```c

```

```c

```

```c

```
