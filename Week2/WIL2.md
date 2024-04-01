# Weekly I Learned - 2

## Github의 기능(source: GitHub Documentation)
### Fork / 포크
>🍴 A fork is a new repository that shares code and visibility settings with the original “upstream” repository.

원하는 리포지토리의 Fork 버튼을 누르면 자신의 GitHub에 새 리포지토리로 추가된다.

다른 사람의 리포지토리를 활용해 자신의 프로젝트를 만들거나, 포크한 리포지토리를 수정하고 원래 소유자에게 풀 리퀘스트를 보내 프로젝트에 기여할 수 있다.

### Star / 스타
>🌟 You can star repositories and topics to keep track of projects you find interesting and discover related content in your news feed.

관심있는 리포지토리의 Star 버튼을 누르면 자신의 프로필에 있는 Stars탭에서 확인할 수 있다. 리스트를 만들어 스타한 리포지토리들을 분류할 수도 있다.
### Issue / 이슈
>🚨 GitHub Issues are items you can create in a repository to plan, discuss and track work.   

Issue는 작업을 추적할 때, 피드백을 주고받을 때, 토의하고 협업할 때, 효율적으로 소통할 때 다양하게 쓰인다.

GitHub 리포지토리의 Issues 탭에서 이슈를 만들 수 있다. 각각의 이슈는 작업자, 레이블, 프로젝트, 마일스톤을 설정할 수 있다.

이슈를 풀 리퀘스트에 연결함으로써 이슈에 대해 작업 중이라는 것을 나타낼 수 있다. 이때 풀 리퀘스트가 머지하면, 자동으로 연결된 이슈가 닫힌다.

### Pull Request / 풀 리퀘스트
>🪢 Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub.

풀 리퀘스트는 브랜치를 병합하늗 데 쓰인다. 새로운 변경을 제안하고 머지할 때 발생하는 충돌을 해결하거나, 머지하기 전 코드에 대해 리뷰하고 토론할 수 있다.

리포지토리 내의 Pull requests 탭에서 만들 수 있다.

## 분기 관리하기

### Branch / 브랜치

브랜치를 만들어 분기하면 다양한 버전의 코드를 관리할 수 있다.

```powershell
$ git branch
#로컬 브랜치 확인
$ git branch "<생성할 브랜치의 이름>"
#브랜치 생성
$ git branch -a
#모든 브랜치 확인
$ git branch -D "<제거할 브랜치의 이름>"
#브랜치 제거, 현재 브랜치는 제거할 수 없음
$ git checkout "<이동할 브랜치의 이름>"
#브랜치 이동
$ git checkout -b "<생성하고 이동할 브랜치의 이름>"
#브랜치 생성 후 이동
```
브랜치의 이름을 정할 때에 암묵의 룰이 있다.

    type/<issue 번호>-<간략한 설명>


### Merge / 머지 / 병합

#### 머지의 3가지 방법
1. Merge Commit

두 브랜치를 공통 부모로 하는 새로운 커밋을 만들어 병합한다.

2. Squash and Merge

브랜치의 커밋 여럿을 하나로 묶어 다른 브랜치로 병합한다.

3. Rebase and Merge

브랜치의 커밋들의 base를 재설정한다.

commit hash가 변경되고, 잘못하면
충돌이 많다고 한다.

아직 이부분은 이해가 잘 되지 않아 나중에 시도해 봐야겠다.

<https://github.com/heonwoos/2024-1-Beginner-Study/issues/1>