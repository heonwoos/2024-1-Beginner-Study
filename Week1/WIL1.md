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
### 4. Commit 팁
무엇을 수정한지 알기 쉽도록 수정 Type을 작성해본다.

> **feat**: 새로운 기능을 추가한 경우   
> **refactor**: 기존 코드를 개선한 경우   
> **fix**: 버그를 수정한 경우   
> **chore**: 코드 외의 설정을 바꾼 경우   
> **docs**: 문서화   
> **test**: 테스트 코드

### 5. 마크다운(Markdown) 연습

```markdown
마크다운에서 마크다운 코드를 적다
# 헤딩
## h2
### h3
###### h6

<hr/>

1. 이
2. 것
3. 은
4. ordered

- 이
    * 것
        + 은
            - unordered and indented

> "이것은 BlockQuote이다"   
> \- Elon Musk


    this is code block   
    

~~*벌써* **코딩이** _귀찮_ __아요__~~

[링크][id]

[id]: [https://www.wikiwand.com/en/Link_(The_Legend_of_Zelda)]
```
#### 위의 마크다운 코드는 다음을 작성한다:

> 마크다운에서 마크다운 코드를 적다
># 헤딩
>## h2
>### h3
>###### h6
>
> <hr/>
>
> 1. 이
> 2. 것
> 3. 은
> 4. ordered
>
> - 이
>     * 것
>         + 은
>               - unordered and indented
> 
> > "이것은 BlockQuote이다"   
> > \- Elon Musk
> 
> 
>       this is code block   
>     
> 
> ~~*벌써* **코딩이** _귀찮_ __아요__~~
>
>
> [링크][id]
> 
> [id]: [https://www.wikiwand.com/en/Link_(The_Legend_of_Zelda)]

### 6. 궁금한 점
1. .md 파일의 경우 어떤 커밋 타입을 써야하는가?
2. 실수한 커밋은 수정할 수 없나?


<https://github.com/Heonwoos/Heonwoos>