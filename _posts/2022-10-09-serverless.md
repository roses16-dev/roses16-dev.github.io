---
layout: single
title: "서버리스 ( Serverless )"
categories: CS
tags: Serverless 
toc: true
sidebar:
  nav: "docs"
---

서버리스 ( Serverless ) 는 서버가 없는 것처럼 Application을 실행할 수 있는 환경을 의미한다.



#### 개요

---

클라우드 컴퓨팅 실행 모델 중 하나로 클라우드 제공자가 동적으로 자원을 할당/관리하여 사용자가 서버를 직접 관리할 필요가 없다.

사용량에 따라 자원을 동적으로 할당하므로 실제 사용 자원에 대한 요금 청구가 가능하여 기존의 종량제 방식보다 경제적이다.





#### 구분 

---

- **Faas ( Function as a service )**

  작성한 코드가 업로드되면 서버는 코드를 함수단위로 쪼개어 대기시킨 후 클라이언트의 요청이 있을 때 함수단위로 실행하여 처리한다. 

  함수 호출 횟수에 따라 비용이 청구된다. 

  - 대표적인 서비스 : AWS Lambda, MS Azure Function 

- **Baas ( Backend as a service )**

  서버리스 서비스 제공자가 백엔드 개발에 필요한 기능을 API형태로 제공하는 서비스이다.

  - 대표적인 서비스 : Firebase





#### 장/단점

---

- 장점
  - 실제 사용량에 대해서만 청구되므로 비교적 경제적이다.
  - 서버에 대한 부담없이 APP 품질에만 집중할 수 있다.
  - 자원이 클라이언트의 요청량에 따라 동적으로 할당되므로 스케일링( 트래픽을 관리하여 병목현상을 예방하는 방법 )에 신경쓰지 않아도 된다.
- 단점
  - Cold Start : 요청이 있을 때에만 동작하기때문에  종량제 방식 보다 비교적 느리다.
  - 함수가 1회 호출될 때 사용가능한 컴퓨팅 자원과 시간에 제한이 있어 긴 시간 작업(동영상 업로드, 데이터백업 등)에는 비효율적이다. 
  - 플랫폼 간 표준화된 지원 방식이 정해져있지 않아 플랫폼을 변경해야할 경우 구조 자체를 바꿔야한다.
    때문에 플랫폼에 종속적인 관계가 된다.





#### 출처

> - https://blog.naver.com/ksyrang/222851443217
