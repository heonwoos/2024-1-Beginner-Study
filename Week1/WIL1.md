# Weekly I Learned - 1

### 0. 깃(git)은 무엇인가?
깃은 버전 관리와 협업을 위한 툴이다.

### 1. 파일의 생명주기

##### Untracked
- Untracked
##### Tracked
- Unmodified
- Modified
- Staged

### 2. git의 영역
1. Working Directory
현재 사용하고 있는 내 컴퓨터의 로컬 폴더이다.

2. Staging Area
커밋하기 전 스테이징을 한다.

3. Local Repo
내 컴퓨터의 리포지토리이다.

4. Remote Repo
외부의 리포지토리이다. github에 생성한 리포지토리가 한 예이다.

### 3. git 명령어와 활용

```powershell
git init
#현재 디렉토리에 .git 폴더를 만든다.

git add .
# 현재 디렉토리의 모든 파일을 스테이징한다.

git commit -m "커밋해야지"
# "커밋해야지"라는 메시지와 함께 로컬 리포지토리에 커밋한다.

git remote add origin <github 주소>
git branch -M main
git push -u origin main
#Remote Repo인 github에 푸시한다.
```