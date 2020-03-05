---
title: Git/GitHub 입문 (oss개발자포럼 세미나)
date: '2019-03-23T13:42:40.000Z'
tags: Seminar
---

# Git/GitHub 입문 \(oss개발자포럼 세미나\)

## Git

![ossgit](https://github.com/cyr9210/Devlog/tree/9a934dfcd84f0e5dd4ab8b4b841fefa9105f1d3b/images/git/ossgit02.png) 버젼관리 시스템인 Git에 대하여 생활코딩 '지옥에서 온 git'을 수강하며, 공부를 하던중...  
oss개발자 포럼 커뮤니티와 국민대학교가 주관하는 'Git과 Github을 이용한 버전관리 입문'이라는 주제로 강연을 진행하단다는 정보를 알게되었습니다. 해당 커뮤니티에 대한 궁금함과 동시에 오프라인으로 강의를 들어보는게 나쁘지 않을것 같아서 신청하게 되었습니다.🙂

### 형상 관리와 버전 관리

#### 형상 관리

**소프트웨어의 변경사항을 체계적으로 추적하고 관리, 통제하는 것**

* 관리대상
  * 요구사항 명세서
  * 설계서
  * 소스코드
  * 이미지
  * 라이브러리 파일
  * 프로젝트 회의록
  * 그외많은관리대상들

#### 형상관리를 왜 해야할까?

* 소프트웨어 개발 생산성을 향상시켜 준다
* \(요구사항을 바탕으로 개발을 진행하므로\) 소프트웨어의 품질을 향상시켜 준다
* \(문제가 있는 경우를 쉽게 발견할 수 있으므로\) 유지보수 비용을 절감시켜 준다

### 버전 관리 시스템

![gitoss](../../.gitbook/assets/ossgit03.png) 소스코드의 변경사항을 체계적으로 추적하고 관리, 통제하는 시스템

#### 버전 관리 시스템 - VCS\(Version Control System\)

![gitoss](../../.gitbook/assets/ossgit04.png)

* 로컬에서 직접 모든 자원을 관리
* USB, 메일 첨부파일

#### 집중형 버전 관리 시스템 - CVCS\(Centralized VCS\)

![gitoss](../../.gitbook/assets/ossgit05.png)

* 하나의서버를두고서버를중심으로모든자원을관리 
* SVN - [https://subversion.apache.org/](https://subversion.apache.org/)

#### 분산형 버전 관리 시스템 - DVCS\(Distributed VCS\)

![gitoss](../../.gitbook/assets/ossgit06.png)

* CVCS처럼 서버를 두고 서버에서 자원 관리를 하지만 로컬에서도 자원 관리를 함
* Git - [https://github.com/git/git](https://github.com/git/git) 

### Git / Github

![gitoss](../../.gitbook/assets/ossgit07.png)

* Git : 버전관리 시스템
* Github : Git 호스팅 사이트

  > 호스팅 : 웹의 공간을 빌려주거나 빌리는것

### Git Hosting

* GitHub \( [https://github.com/](https://github.com/) \) 
* GitLab \( [https://gitlab.com](https://gitlab.com) \) 
* BitBucket \( [https://bitbucket.org](https://bitbucket.org) \)

  **Git Client**

* Git bash
  * Git을 설치하면 기본제공되는 CLI 기반 Git Client
  * Windows / Mac / Linux

    SourceTree

  * [https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/)
  * Windows / Mac

    GitKraken

  * [https://www.gitkraken.com/](https://www.gitkraken.com/) - Windows / Mac / Linux

### Git을 이용한 버전 관리

* 버전관리 ⊂ 형상관리
* Git은 분산형 버전 관리 시스템\(DVCS\) Git ≠ GitHub
  * GitHub는 Git Hosting 웹 서비스

#### 버전관리를 어떻게할까?

* CVCS
  * ![gitoss](../../.gitbook/assets/ossgit08.png)
  * ![gitoss](../../.gitbook/assets/ossgit09.png)
* DVCS
  * ![gitoss](../../.gitbook/assets/ossgit10.png)
  * ![gitoss](../../.gitbook/assets/ossgit11.png)
* Git\(DVCS\)
  * ![gitoss](../../.gitbook/assets/ossgit12.png)

#### Git의 흐름\(workflow\)

![gitoss](../../.gitbook/assets/ossgit13.png) ![gitoss](../../.gitbook/assets/ossgit14.png)   
  


### GitHub 둘러보기

* fork : 다른사람의 프로젝트를 복제
* Pull Request : 자신이 변경한 코드를 상대방의 리포지토리에 넣고 싶을 때 사용하는 기능
  * git Lab에서는 merge request라고 부른다.
  * Pull Request에도 순서가 있다.

    ![gitoss](../../.gitbook/assets/ossgit15.png)
* git fetch : 리포지토리에서 변경된 기록을 가져오되 merge는 하지 않음
* git pull : 리포지토리에서 변경된 기록을 가져오고 merge도 바로 이루어짐

### 알아두면 좋은것

* [생활코딩 지옥에서 온 Git](https://opentutorials.org/course/2708)
* [동네개발자형 교육방송 - git bisect](https://www.youtube.com/watch?v=SYVUyNrQhAU)
* 여러 프로젝트, 소식 살펴보기 : [gitexplore](https://github.com/explore)
  * 오픈소스 fork시, [라이센스](https://opensource.org/licenses)에 주의해야한다.   

    참고자료 : [https://www.slideshare.net/ssuser22e7fc/gdg-campus-korea-2-132342619](https://www.slideshare.net/ssuser22e7fc/gdg-campus-korea-2-132342619)
* [gitignore 적용하기](http://www.itpaper.co.kr/gitignore-%ED%8C%8C%EC%9D%BC%EC%9D%84-%E%20D%86%B5%ED%95%9C-%EB%AC%B4%EC%8B%9C%EB%AA%A9%EB%A1%%209D-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0/)
  * [gitignore.io](https://www.gitignore.io/)
* 참고하면 도움이 될 책
  * 소프트웨어 개발의 모든 것
  * 성공으로 이끄는 팀 개발 실천 기술
  * 팀을 위한 git

### 명령어

* git 사용자 정보 조회
  * git config --global --list
* 이전에 git을 사용한 적이 있다면 사용자 정보를 지워줍니다.
  * git config --global --unset-all user.name
  * git config --global --unset-all user.email

강의는 매우 만족스럽지 못했습니다.. 발표자는 20분이 넘는 시간을 지각하고, wifi접속은 안되고, 강의내용은 기존 공지내용과 달랐습니다. bash기반의 명령어 및 구동원리 강의를 기대하고 왔는데..  
해당 강연은 git 크라켄을 사용하는 gui방식의 툴을 기반으로 하고 있었으며, git에대해 전혀 알지못하는 사람을 대상으로 하는 수준이었기 때문에 제가원하는 강연은 아니었던것 같습니다. 분명 강의내용에 명령어 강의라고 되어있어서 신청했는데..😂 git을 처음접하시는 분들에게는 어땠을지 모르겠지만 제게는 많이 아쉬웠던 강의였습니다.   
  


