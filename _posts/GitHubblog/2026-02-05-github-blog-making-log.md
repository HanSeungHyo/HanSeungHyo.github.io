---
title: "깃허브 블로그"
date: 2026-02-05
categories: [GitHubblog]
tags: [github-pages, jekyll, blog]
slug: github-blog-first
---

아니 대충했다고 포스팅이 다 하나로 통일되고 있네
slug: github-blog-first추가함 이걸로 분리가능하데 근데 퍼스트가 아니잖아e: "깃허브 블로그"
date: 2026-02-05
categories: [GitHubblog]
tags: [github-pages, jekyll, blog]
slug: github-blog-first
---

아니 대충했다고 포스팅이 다 하나로 통일되고 있네
slug: github-blog-first추가함 이걸로 분리가능하데 근데 퍼스트가 아니잖아

대충 방치한지 5일 됬다

더 귀찮아서 안쓰기 전에 일단 암거나 쓰면 나중에 수정하겠지라는 마음으로 쓰기
이때도 귀찮아서 안쓰기전에 쓰겟지했는데 손도 안됨

아 너무 귀찮아

자꾸 커밋하면 잔디가 안심겨서 슬퍼서 잔디 심고싶어서 찾아댕기다가 
원인을 찾았다

일단 내가 컴퓨터랑 이메일 연동을 안해서 안뜨는 줄 알았는데 포그할때마다 잔디찍히는거보면 그건아니여서
계속 찾아봄

그러던 중
포그한 템플릿같은거는 안될수있다는겨

그래서 일단 테스트를 했는데 저 테스트 저장소를 보면 바로 잔디가 찍혀잇는게 보이는데

계정 잔디 시스템은 정상
커밋도 정상적으로 잔디 찍힘
문제는 블로그 저장소(HanSeungHyo.github.io) 쪽 커밋이 잔디 집계에서 빠지는 것

1️⃣ Pages 저장소 커밋은 “기여”로 덜 잡히는 경우 있음

특히
설정 파일 수정(_config.yml)
테마 파일 복붙
자동 생성 파일
GitHub에서 만든 커밋
이런 건 잔디에 누락되는 경우 많음.

2️⃣ 커밋 author/email 정보가 애매하게 기록됨
너가 말했듯이
블로그 repo 커밋에는 이메일 줄이 안 떴다
이게 핵심이야.
GitHub가 커밋은 인정하지만
Contribution graph에 연결을 안 해주는 거지.

3️⃣ GitHub Actions/Pages 배포 커밋은 잔디에 안 찍힘

블로그는 내부적으로
build
deploy
자동 작업이 섞여서
봇 커밋처럼 처리되기도 함.


✅ test repo 만드는 방법
1️⃣ GitHub 들어가기
오른쪽 위에 + 버튼 있지?
거기서
👉 New repository 클릭
2️⃣ 저장소 이름 적기
예를 들어:
test-contribution
아무 이름이나 상관없어.

3️⃣ 설정은 이렇게
✅ Public 선택
✅ 아래 체크

☑️ Add a README file
이거 꼭 체크!

4️⃣ Create repository 버튼 누르기
그러면 저장소가 바로 생성됨.

✅ 커밋 하나 만들어서 잔디 심기
README.md 열기

파일이 자동으로 생겨있을 거야.

오른쪽 위에 ✏️ (Edit) 버튼 누르기

내용 아무거나 추가해

예:
잔디 테스트용 커밋입니다.
아래로 내려서 Commit 하기
Commit message:
test commit


그리고

✅ Commit directly to the main branch 선택

마지막으로

👉 Commit changes 버튼 클릭

🎯 결과는 이렇게 봐야 함

이 커밋이 내일 잔디에 찍히면 → 계정은 정상

이것도 안 찍히면 → Contribution 설정 문제

그래서 잔디를 심게하는거

Settings > General > Leave fork network
원본업데이트를 못받지만 잔디는 심긴다

하나는 복사한 커밋을 붙여넣을 레포지토리를 생성해서 어찌하는건데
그냥 원본업데이트를 끊었다

https://hadahae2024.tistory.com/11
이러한 잔디꾸미기도있는데

토큰이 공개되면 프로필용 토큰은 프로필 레포지토리 수정 권한을 가질수있다는 걸 배우고 2차 보안에 힘쓰기로했다

authenticator 앱으로 2차보안이 가능하다는 
