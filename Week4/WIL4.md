# Weekly I Learned - 4

## 브랜치 관리 방법

### 1. Git Flow


#### Main Branches
- main(혹은 master)
    1. 프로젝트 최초의 브랜치
    2. 삭제되지 않음

- develop
    1. main 생성 후 두번 째로 생성하는 브랜치
    2. feature 브랜치를 분기하는 베이스

#### Supporting Branches
- feature
    1. develop 브랜치에서 분기하는 브랜치
    2. 기능을 개발하고 나서 develop에 merge함
    3. main, master, develop, release, hotfix를 제외한 이름으로 지음
- release
    1. 배포를 위한 브랜치
- hotfix

### 2. GitHub Flow
