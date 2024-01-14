---
title: Git 브랜치 main과 master 차이
date: 2023-12-15 15:20:00 +0800
categories: [ect.]
tags: [Git, main, master, Branch, github]
---

## **Git master와 main 브랜치란?**

master 브랜치는 기존에 git에서 사용되던 기본 브랜치이다.

현재는 main 브랜치를 기본 브랜치로 권장하고 있으나 master 브랜치를 그대로 사용하여도 무방하다.

하지만 Github에서 main을 기본 브랜치로 제공하고 있어 새로운 프로젝트를 구축한다면 main 브랜치 사용을 권장한다.

---

> **왜 main을 권장할까?**  
> 블랙 리브스 매터(Black Lives Matter, 흑인 생명은 소중하다) 운동으로 인해master 브랜치를 main 브랜치로 이름을 변경하였다.
> 인종차별 반대라는 의미가 있는 변경인 것이다.  
{: .prompt-info }

## **git 기본 브랜치 변경하기**

git을 사용하다 보면 github 기본 브랜치와 git 기본 브랜치명이 달라서 불편함이 생기기도 한다.

불편함을 해소하기 위해 git 기본 브랜치를 main으로 변경하는 방법은 아래와 같다.

#### **1\. git 버전 확인하기**

```
$ git --version
```

#### **2\. global gitcofig 설정하기**

```
$ git config --global init.defaultBranch main
```

#### **3.defalutBranch 확인하기**

```
$ git config --get  init.defaultBranch
```
