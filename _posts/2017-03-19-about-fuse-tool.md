---
layout: post
title: "Fuse 간단 조사"
tags: [Fuse]
comments: true
---

- Fuse 소개(다른 자료로 대체)
  - Fuse 기본적인 기능들에 대한 guide
    - https://www.fusetools.com/docs/basics/feature-overview
- 현재 fuse로 어느 수준까지 개발이 가능한가?
  - 프로토 타이핑에는 이만한 Tool이 없을듯
  - 내부적으로 OpenGL을 Base로 모든 그래픽을 구현하기 때문에 빠르고 자연스럽고 사용하기 편하다
  - Business Logic은 javascript를 이용한다. UI랑 Business Logic을 얼마나 분리할 수있을지는 아직 잘 모르겠다.
- Fuse 코드 구조 파악 및 안드로이드와 코드 구조 비교
  - Fuse Code
  - Android Code
- Fuse 개발 채택 시 발생할 장/단점
  - 장점
    - 초기 프로토타입은 굉장히 빠른 시간에 나올 수 있음
    - Local에서 Preview tool을 통해 코드 수정하고 바로 결과 확인이 가능. Mobile App개발하다 보면 조금만 수정해도 새로 빌드하고 확인해야 하는데 이건 그냥 실시간 반영. 최대의 장점이다
    - iOS의 경우 OS버전별 파편화가 크지 않지만 안드로이드는 파편화가 너무 커서 이거 대응하는데도 꽤 많은 시간을 들여야함. Business Logic엔 그런 부분이 없지만 UI처리는 SupportLibrary를 쓰는 등 은근히 신경써야 하는 부분이 많음. 그런데 Fuse는 OpenGL로 그래픽을 다 처리하기 때문에 이런 부분에서 자유롭다.
    - Animation 사용이 굉장히 편함
- 단점
  - 기본적인 View들은 예제를 통해 제공하지만
  - 떼루바 특성상(채팅) 항상 Network를 항상 사용하는데, fuse가 Network 처리에 얼마나 성숙도가 높은지 아직 검증되지 않았다.
