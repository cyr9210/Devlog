---
title: HotelReservation-System(DB Mini project)
date: '2018-12-07T21:05:09.000Z'
tags: 프로젝트_회고
---

# HotelReservation-System\(DB Mini project\)

## DataBase Mini Project

### HotelReservation-System

**Project github :** [https://github.com/cyr9210/Hotel-Reservation\_System](https://github.com/cyr9210/Hotel-Reservation_System)

#### 구현내용

![HotelReservation](../../.gitbook/assets/hotelreservation01.png) ![HotelReservation](../../.gitbook/assets/hotelreservation02.png) ![HotelReservation](../../.gitbook/assets/hotelreservation03.png)

* 저희팀의 DB 실기평가를 위한 미니프로젝트의 주제로 숙박어플 여기어때를 벤치마킹한 숙박업소 예약 DB를 선택하였습니다.

![HotelReservation](../../.gitbook/assets/hotelreservation04.png)

* 각자 스마트폰에 어플을 설치하여 요구사항분석을 진행하였습니다.
* 최초의 요구사항분석은 보다 많이 나열하였으나, 2일이라는 짧은 시간과 현재 우리가 만들 수 있을 내용들을 선택하여 재구성하였습니다.

![HotelReservation](../../.gitbook/assets/hotelreservation05.png) ![HotelReservation](../../.gitbook/assets/hotelreservation06.png) ![HotelReservation](../../.gitbook/assets/hotelreservation07.png) ![HotelReservation](../../.gitbook/assets/hotelreservation08.png) ![HotelReservation](../../.gitbook/assets/hotelreservation09.png) ![HotelReservation](../../.gitbook/assets/hotelreservation10.png) ![HotelReservation](../../.gitbook/assets/hotelreservation11.png) ![HotelReservation](../../.gitbook/assets/hotelreservation12.png) ![HotelReservation](../../.gitbook/assets/hotelreservation13.png) ![HotelReservation](../../.gitbook/assets/hotelreservation14.png) ![HotelReservation](../../.gitbook/assets/hotelreservation15.png) ![HotelReservation](../../.gitbook/assets/hotelreservation16.png)

* 중복된 속성값들을 분류

![HotelReservation](../../.gitbook/assets/hotelreservation17.png)

* ‘예약번호’ 를 주식별자로 가지지 않는 속성들을 분리

![HotelReservation](../../.gitbook/assets/hotelreservation18.png)

* 회원등급이라는 일반속성과 그 속성을 키값으로 가지고 분류될수 있는 적립률을 분리

![HotelReservation](../../.gitbook/assets/hotelreservation19.png)

* 데이터를 입력하기 위해 각 엔티티들의 관계를 설정하여 E-R Diagram 을 작성하였습니다.

![HotelReservation](../../.gitbook/assets/hotelreservation20.png) ![HotelReservation](../../.gitbook/assets/hotelreservation21.png) ![HotelReservation](../../.gitbook/assets/hotelreservation22.png)

* ‘예약목록' 테이블의 경우, 숙소의 방번호 와 입실날짜가 중복되어 예약될 수 없기 때문에 PRIMARY KEY의 인자로 방번호와 입실일을 선택

![HotelReservation](../../.gitbook/assets/hotelreservation23.png) ![HotelReservation](../../.gitbook/assets/hotelreservation24.png)

* SELECT문을 활용하여 회원명 및 회원등급을 조회

![HotelReservation](../../.gitbook/assets/hotelreservation25.png)

* 회원 측에서 요청될 수 있는 회원번호로 예약현황 조회를 구현   

  \(JOIN활용\)

![HotelReservation](../../.gitbook/assets/hotelreservation26.png)

* 서브쿼리문을 활용하여 가장 싼 숙소 TOP3를 조회   

  \(FROM절 서브쿼리문 활용\)

![HotelReservation](../../.gitbook/assets/hotelreservation27.png)

* 호텔 전체 평균 평점보다 평점이 높은 숙소 검색   

  \(서브쿼리문 활용\)

![HotelReservation](../../.gitbook/assets/hotelreservation28.png) ![HotelReservation](../../.gitbook/assets/hotelreservation29.png)

* PL/SQL을 활용하여 SQL내에서 예약기능을 구현   

  \(DUP\_VAL\_ON\_INDEX\(무결성위배\) 예외발생 시, ROLLBACK 하도록 예외처리 하였습니다.\)

![HotelReservation](../../.gitbook/assets/hotelreservation30.png)

* 앞서 만들었던 PL/SQL을 PROCEDURE로 만들어 EXECUTE문 활용하여 실행

![HotelReservation](../../.gitbook/assets/hotelreservation31.png)

### 느낀점

2일동안 조원들과 고민하고 고민하여 미니프로젝트를 완성하였다. 프로젝트를 진행하며 앞서 배웠던 내용들을 복습할 수 있는 시간이되어 좋았다. 데이터모델링을 하는 부분이 가장 어려웠는데, 각 엔티티들의 관계설정이 가장 어려웠다. 진행하면서 데이터 모델링 부분이 정말 어렵고 현 실무자들은 데이터들의 검색속도 및 성능들까지 정말 대단하고 어서 빨리 취업하여 배우고 싶다는 생각을 하였다. 부족한 결과물이지만, 나는 개인적으로 부족한 부분을 복습도 할 수 있었고, E-R Diagram을 작성하며 관계부분을 이해하는데 도움이되어 만족스러웠다.   
  


