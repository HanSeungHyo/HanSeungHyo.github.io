---
title: "피보나치 수열을 해보자"
date: 2026-04-01
categories: [GitHubblog]
tags: [github-pages, jekyll, blog]
slug: github-blog-first
---

정처기를 풀다가 

#include <stdio.h>

int main() {
    int a[10];
    a[0] = 0;
    a[1] = 1;

    for (int i = 0; i < 8; i++) {
        a[i + 2] = a[i + 1] + a[i];
    }

    printf("%d", a[9]);
}
