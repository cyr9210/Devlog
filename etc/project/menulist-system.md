---
title: MenuList System(Java Mini Project)
date: '2018-11-23T15:06:23.000Z'
tags: 프로젝트_회고
---

# MenuList System\(Java Mini Project\)

## Java Mini Project

### MenuList\_System

**Project github :** [https://github.com/cyr9210/Menu-List-System](https://github.com/cyr9210/Menu-List-System)

#### 구현내용

![MenuList](../../.gitbook/assets/menulist_system01.png) ![MenuList](../../.gitbook/assets/menulist_system02.png) ![MenuList](../../.gitbook/assets/menulist_system03.png) ![MenuList](../../.gitbook/assets/menulist_system04.png) ![MenuList](../../.gitbook/assets/menulist_system05.png) ![MenuList](../../.gitbook/assets/menulist_system06.png) ![MenuList](../../.gitbook/assets/menulist_system07.png) ![MenuList](../../.gitbook/assets/menulist_system08.png) ![MenuList](../../.gitbook/assets/menulist_system09.png) ![MenuList](../../.gitbook/assets/menulist_system10.png) ![MenuList](../../.gitbook/assets/menulist_system11.png) ![MenuList](../../.gitbook/assets/menulist_system12.png) ![MenuList](../../.gitbook/assets/menulist_system13.png) ![MenuList](../../.gitbook/assets/menulist_system14.png) ![MenuList](../../.gitbook/assets/menulist_system15.png) ![MenuList](../../.gitbook/assets/menulist_system16.png) ![MenuList](../../.gitbook/assets/menulist_system17.png)

#### 상세설명

![MenuList](../../.gitbook/assets/menulist_system18.png)

* Customer\(고객\) 와 Admin\(관리자\)는 추상 클래스 User를 상속받는다.

![MenuList](../../.gitbook/assets/menulist_system19.png) ![MenuList](../../.gitbook/assets/menulist_system20.png)

* User는 추상메소드 showMenu를 가지고, Customer 및 Admin은 showMenu를 오버라이딩 한다.
* Customer 와 Admin에는 각각의 기능들을 구현할 수 있는 일반 메소드를 가진다.

![MenuList](../../.gitbook/assets/menulist_system21.png)

* MenuManager 클래스는 Menu객체를 ArrayList를 담는다.
* Menu는 4개의 String 변수를 갖는다.

![MenuList](../../.gitbook/assets/menulist_system23.png)

* Manager 클래스는 생성한 클래스들을 객체화한다.
* 생성한 객체들을 상호작용하여 요구하는 기능들을 구현하는 메소드를 가진다.

![MenuList](../../.gitbook/assets/menulist_system24.png)

* Main클래스는 Manager클래스에서 구현한 메소드 기능들을 불러온다.

### 느낀점

우리조도 나름 잘 구현했다고 생각했는데, 다른 조들의 발표내용들을 보고 너무 잘해서 놀랐다. 이번 프로젝트의 가장 아쉬운점은 접근제어자를 사용하지 않고 대부분 default 상태로 접근을 제어하였다는것이다. get /set 메소드를 많이 사용한만큼 해당변수들에 대해 private 접근제어자를 설정했어야 됬다고 생각한다. 시간이 많이 없었던 탓인지 정신없이 하다보니 놓친것 같다. 이번 프로젝트를 통해 정말 많이 부족함을 느끼고 더 열심히 배우고 많은 반복 복습이 필요할 것 같다.   
  


