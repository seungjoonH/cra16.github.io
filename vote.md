---
layout: page
permalink: /vote/
title: Vote
tags:
image:
  feature: abstract-3.jpg
  credit:
  creditlink:
share: true
---

# 삼성 SDS 「S/W 동아리 Championship」

CRA는 이번 제 3회 삼성 SDS 「S/W 동아리 Championship」에 참가하고자 합니다. 두 팀이 참가하기를 희망하고 있으나, 하나의 팀만 참가할 수 있는 관계로 동아리원 투표로 결정하고자 합니다. 아래 각 팀별 주제를 읽어보시고 카카오톡 동아리 공지방에서 투표를 해주시길 바랍니다.

## 1. Overcast 클라우드 컴퓨팅 시스템

![Overcast-Overview](/images/overcast-1.png)

### 문제 정의

매 학기 많은 개발 프로젝트가 학부 안에서 진행된다. 모바일 앱이나 웹 서비스 프로젝트가 많아진 최근 경향에 따라 서비스에 사용할 백엔드(_back-end_) 서버의 수요도 높아지는 추세이다. 그러나 개인이 소지한 PC에 서비스를 위한 웹서버를 설치하는 과정은 오버헤드가 크다. 개인 PC에 서버를 운영하면 언제나 온라인 상태임을 보장하지 못하기 때문에 프로젝트의 다른 구성원이 서버에 접근할 때마다 PC 소유자에게 서버 온라인 여부를 확인해야 하는 상황이 빈번하게 발생한다. 프로젝트를 여러 번 겪었던 사람의 경우 소유한 PC에 여러 버전의 웹서버가 설치되어 포트 중복이나 설정 충돌 문제 등으로 실제 프로젝트를 진행할 때 의도치 않은 문제점이 발생하기도 한다. 장기간 진행하는 프로젝트나 실제 서비스에 들어가는 웹 서비스의 경우 백엔드 서버를 별도로 구매할 필요가 생기지만 꾸준한 관리가 어렵고 하드웨어 고장의 위험성 때문에 호스팅 서비스를 이용하는 경우가 많다. 하지만 유료 서비스의 경우 비용의 문제, 무료 서비스의 경우 시스템 성능 전송량 등의 제약 조건이 걸려 있어 학생들에게 많은 부담을 안겨준다.

### 개발 동기

CRA에서 보유한 하드웨어 자원들을 효율적으로 사용할 방법은 없을까 고민했던 것이 Overcast 개발 동기의 시초가 되었다. 사용할 수 있는 서버는 많지만 실제로 사용하는 서버는 i7 서비스 서버와 CRA 테스트 서버뿐이어서 나머지 서버의 자원이 낭비되는 실정이었다. 이에 클라우드 운영체제와 네트워크 가상화 기술을 도입해 물리적으로 분리된 서버를 논리적 구성망으로 통합, 동아리에서 사용되지 않고 낭비되는 서버 유휴 자원으로 IaaS를 구현하여 하드웨어 자원을 유용하게 활용해보고자 했다.

처음에는 단순하게 동아리 안에서만 쓰이는 시스템을 구축할 계획이었지만, 담당 교수님과의 회의, 내부 의견을 통해, 단지 동아리 안에서만 쓰이는 것을 넘어서, 한동대 구성원들에게 사설 클라우드 컴퓨팅 서비스를 제공할 수 있도록 규모를 확장해 보자는 것에 의견을 모았다.

### 목적

웹 인터페이스를 통해 인스턴스(_instance_)을 손 쉽게 생성할 수 있는 클라우드 시스템을 제공한다. 인스턴스는 전가상화(_full-virtualization_) 기술을 통해 빠른 응답 속도와 성능을 가지고 있으며 루트 권한 부여로 사용자에게 완전한 제어권을 제공한다. 특정 서비스를 이용하려는 사용자에게는 미리 정의된 템플릿을 제공하여 Apache HTTP Server, PHP, MySQL 등의 서비스 스택이 설치되어 있는 상태의 인스턴스를 몇 분 내로 생성하여 제공한다. 각 인스턴스에 연결되는 부팅 볼륨은 저장소(_storage_) 서비스에서 용량를 선택 후 생성하여 일반적인 하드디스크처럼 사용할 수 있으며, 스냅샷(_snapshot_) 기능을 통해 저장소 볼륨의 백업을 생성하여 장애 상황 발생 시 빠르게 복원 작업을 할 수 있다. 하드웨어 가상화 기술을 적용하여 단기간 운용하는 프로젝트 서버뿐 아니라 실제 서비스하는 백엔드 서버도 고가용성을 보장하며 안정적으로 가동할 수 있는 서비스를 제공하고자 한다.



## 2. Kinect와 영상인식을 이용한 어린이 놀이 재해석

![키넥트x숭익](/images/kinect-x-monkey.jpg)
