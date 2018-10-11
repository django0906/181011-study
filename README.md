# 181011-study

## Contents
#### 1. 무슨 프로젝트인가?
##### 1.1 환경설정
##### 1.2 디렉토리 구조
#### 2. 현재까지 한 일
#### 3. 앞으로 할 일

---

#### 1. 무슨 프로젝트인가?

기존의 django-vagrant-1st-project를 처음부터 다시 손대봅니다.

Django를 사용한 소규모 커뮤니티 사이트를 만들 프로젝트입니다.

##### 1.1 환경설정

* Darwin rgpkoreaui-MacBook-Pro-6.local 17.7.0 Darwin Kernel Version 17.7.0: Thu Jun 21 22:53:14 PDT 2018; root:xnu-4570.71.2~1/RELEASE_X86_64 x86_64
* PostgreSQL 9.6
* Virtualenv로 pip 관리를 수행했습니다.
    * 상세 내용은 requirements.txt를 참조 바랍니다.

##### 1.2 디렉토리 구조
```
django_small_bbs_project/
    .gitignore
    docs/
    README.md
    requirements.txt
    django_small_bbs/
        bbs/
        config/
        login/
        logout/
        media/
        register/
        static/
        templates/
        manage.py
``` 
* Two Scoops of Django에서 권장하는 디렉토리 방식 도입. 아래의 룰을 따른다.
```
<repository_root>/
    <django_project_root>/
        <configuration_root>/
```
* 앱의 이름과 역할은 다음과 같다:
    * bbs: 로그인한 유저에게 제공하는 게시판 기능
    * login: 로그인 기능
    * logout: 로그아웃 기능
    * register: 회원가입 기능
---

#### 2. 현재까지 한 일

현재까지 수행한 요소는 다음과 같습니다.

* 기본 디렉토리 구조 구축

---

#### 3. 앞으로 할 일

추후 구현해야 할 요소는 다음과 같습니다.

* login/logout/register 구현

* 데이터베이스 구축
    * Django User 사용하기
    * 게시판 기능 추가하기
        * 게시판 모델링하기
        * Many to Many 형태의 queryset 사용해보기
        * 로그인시 index 에 접근하여 게시판 보여주기
        * 게시판 추천/비추천 기능 비동기식 구현하기
        * 비회원도 로그인 및 글 작성이 가능하게 제작하기.
            * 접속자의 IP 주소 앞자리 두자리를 공개하게 하기.
    
* Django Authenticate, Login 사용
    * 비동기 처리 연습하기
    
* [진행중!] Two scoops of Django 1.8 보면서 많은 구조 참조하기
    * 프로젝트 구조 전체 보완하기
    * 1.11버전 책은 필요에 따라 구매
    
