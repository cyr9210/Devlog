---
title: '알고리즘, 반복 (doit-알고리즘)'
date: '2019-03-14T09:59:13.000Z'
tags: Algorithm
---

# 알고리즘, 반복 \(doit-알고리즘\)

![Java](../.gitbook/assets/algorism_logo.png)

## Study

### Algorism

알고리즘 시험을 시행하는 회사들이 많아졌습니다. 시험을 대비하기 위해 매주 조금씩 알고리즘을 공부하기로 마음을 먹었습니다.

알고리즘은 아래 교재로 진행할 예정입니다. 🙂  


![](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/algorithm/images/doit_algorithm.jpg)

### 기본알고리즘

#### 알고리즘

문제를 해결하기 윈한 것으로, 명확하게 정의되고 순서가 있는 유한 개의 규칙으로 이루어진 집합   
  


#### 세 값의 최대값

```text
public void max(){
        Scanner sc = new Scanner(System.in);

        System.out.println("세 정수의 최대값을 구합니다.");

        System.out.print("a : ");
        int a = sc.nextInt();
        sc.nextLine();
        System.out.print("b : ");
        int b = sc.nextInt();
        sc.nextLine();
        System.out.print("c : ");
        int c = sc.nextInt();
        sc.nextLine();

        int max = a;

        if (max < b) {
            max = b;
        }

        if (max < c) {
            max = c;
        }

        System.out.println(max);
}
```

**과정**

1. max에 a값을 넣는다.
2. b값이 max보다 크면 max에 b값을 넣는다.
3. c값이 max보다 크면 max에 c값을 넣는다.

**결과**

![doital](../.gitbook/assets/doital01-01.png)

**학습내용**

* 순차적 구조 : 위와 같이 세 문장이 아래로 나란히 있을 때, 순차적으로 실행되는 구조
* 선택\(Selection\) 구조 : \(\)안에 식의 평가 결과에 따라 프로그램의 실행흐름을 변경하는 if문과 같은 구조

#### 조건 판단과 분기

```text
public void judgeSign(){
        System.out.print("정수를 입력하세요 : ");
        int n = sc.nextInt();

        if (n > 0) {
            System.out.println("양수입니다.");
        } else if (n < 0) {
            System.out.println("음수입니다.");
        }else{
            System.out.println("0입니다.");
        }
}
```

#### 결과

![doital](../.gitbook/assets/doital01-02.png)

#### 순서도의 기호

**프로그램 순서도**

![](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/algorithm/images/doital/doital01-03.png)

* 데이터 : 데이터의 입력과 출력

![](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/algorithm/images/doital/doital01-04.png)

* 처리 : 연산집합이나 연산군의 실행

![](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/algorithm/images/doital/doital01-05.png)

* 미리 정의한 처리 : 서브루틴 및 모듈 등 다른곳에서 이미 정의한 하나 이상의 연산 또는 명령어들로 이루어진 처리

![](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/algorithm/images/doital/doital01-06.png)

* 판단 : 하나의 입구와 하나 이상의 출구가 있고, 정의한 조건을 평가하여 하나의 출구를 선택하는 판단기능

![](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/algorithm/images/doital/doital01-07.png)

* 루프 범위 : 루프의 시작과 종료
  * 루프의 이름 사용\(시작과 종료에 같은값\)
  * 시작 또는 종료 기호에 초깃값, 증갓값, 종룟값 표기
* 선 : 제어의 흐름
  * 흐름의 방향을 분명히 나타내고자 할 때, 화살표를 붙인다. 

![](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/algorithm/images/doital/doital01-08.png)

* 단말 : 외부환경으로 나가거나, 들어오는것을 나타냄
  * ex\)프로그램의 시작과 종료

### 반복

#### 1부터 n까지 정수의 합 구하기, 양수만 입력하

```text
 public void sum(){
        /*무한for문 사용(while(ture)도 마찬가지

        int n;

        for (;;){
            System.out.print("n : ");
            n = sc.nextInt();
            sc.nextLine();

            if(n > 0){
                break;
            }else{
                System.out.println("0보다 큰 숫자를 입력해주세요.");
            }
        }*/


        int n;

        do{
            System.out.print("n : ");
            n = sc.nextInt();
            sc.nextLine();

            if (n <= 0) {
                System.out.println("0보다 큰 숫자를 입력해주세요.");
            }
        }while(n <= 0);


        int sum = 0;

        for (int i = 1; i <= n; i++) {
            sum += i;
        }

        System.out.println(n + "까지 합 : " + sum);
    }
```

**결과**

![doital](../.gitbook/assets/doital01-09.png)

#### 구조적 프로그래밍

하나의 입구와 하나의 출구를 가진 구성 요소만을 계층적으로 배치하여 프로그래밍을 구성하는 방법

* 구조적 프로그래밍을 3종류의 제어흐름을 사용한다.
  * 순차
  * 선택
  * 반복

**논리연산과 드모르간 법칙**

* 단푹평가 : 논리 연산의 식 전체를 평가한 결과가 왼쪽 피연산자의 평가 결과만으로 정확해지는 경우, 오른쪽 피연산자의 평가를 수행하지 않는다.
* 드모르간 법칙 : 각 조건을 부정하고 논리곱을 논리합으로, 논리합을 논리곱으로 바꾸고 다시 전체를 부정하면 원래의 값과 같다.

#### 다중루프

다중루프 반복안에서 다시 반복되는 등의 경우

**곱셉표**

```text
for (int i = 2; i < 10; i++) {
            for (int j = 1; j <  10; j++) {
                System.out.println(i + " x " + j + " = " + i*j);
            }
}
```

**결과**

![doital](../.gitbook/assets/doital01-10.png)

#### 직각 이등변 삼각형 출력

```text
 public void triangleLB(){
        int n;
        System.out.println("왼쪽아래가 직각인 직각 삼각형 출력");

        do{
            System.out.print("n : ");
            n = sc.nextInt();
            sc.nextLine();
        }while (n <= 0);

        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
}
```

**결과**

![doital](../.gitbook/assets/doital01-11.png)

