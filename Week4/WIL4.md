# Weekly I Learned - 4

## 브랜치 관리 방법

### 1. Git Flow

#### 구조
##### Main Branches
- main(혹은 master)
    1. 프로젝트 최초의 브랜치
    2. 삭제되지 않음

- develop
    1. main 생성 후 두번 째로 생성하는 브랜치
    2. feature 브랜치를 분기하는 베이스

##### Supporting Branches
- feature
    1. develop 브랜치에서 분기하는 브랜치
    2. 기능을 개발하고 나서 develop에 병합함
    3. main, master, develop, release, hotfix를 제외한 이름으로 지음
- release
    1. develop 브랜치에서 분기하는 브랜치
    2. 배포할 때 main으로 병합함
    3. 작은 버그를 수정하고 QA 작업을 함
- hotfix
    1. main 브랜치에서 분기
    2. 수정 후 main과 develop 브랜치에 병합함
    3. 배포 환경에서 즉각적인 수정이 필요할 경우 사용

#### 단점
- 짧은 주기로 배포를 한다면 비효율적

### 2. GitHub Flow

#### 구조

- main
    1. 항상 배포 가능 상태로 유지
    2. main으로 병합 전에 충분한 테스트 필요
- feature
    1. main 브랜치에서 분기함
    2. 작업 후 main으로 병합
    3. feature, hotfix, release를 구분하지 않음
    4. 브랜치의 목적을 이름에 잘 담아야 함
    5. Git Flow에 비해 코드 리뷰 중요

## 좋은 개발자의 태도

### Convention 만들기
- 오랜 시간이 지난 후 커밋 또는 브랜치 이름을 보고 바로 의도를 파악할 수 있다.
- 보기 좋아진다.

### 물어보기 전에 구글링 먼저
- 구글에서 대부분의 문제의 해결법을 찾을 수 있다.
- 직접 문제 해결 방법을 찾는 것이 기억에 더 오래 남는다.
- 그래도 모르겠으면 물어보기

### 코드에 대한 주인 의식 가지기
- GitHub는 모두가 내 코드를 볼 수 있다.
- 스파게티 코드 말고 잘 설계된 코드를 짜자.

### 질문을 잘 하자
- 질문을 해야한다면 좋은 질문을 하자.
- 무엇을 모르는지 정확히 알자.