# 💫 Commit을 되돌리는 세 가지 방법 ⏪

## 1. git commit --amend

> **amend** /əˈmend/   
> 뜻: (특히 법적 문서의) 단어 또는 글자를 바꾸다.

#### 1. 
```powershell
$ git commit --amend -m "수정된 커밋 메시지"
# -m 옵션: vim 진입 없이 커밋 메시지를 수정한다
```
#### 2. 
```powershell
$ git commit --amend --no-edit
# --no-edit 옵션: 메시지 수정 없이 커밋 수정
```
> ⚠️주의!   
> 협업자의 작업 기반인 커밋은 amend 하지 말 것

## 2. git reset

- 설정한 커밋 해시의 커밋보다 나중의 커밋을 삭제한다.

### 2.1. --soft
```powershell
$ git reset --soft <커밋 해시>
# 커밋만 삭제(Staging Area에 그대로)
```

### 2.2. --mixed (기본값, 생략 가능)
```powershell
$ git reset --mixed <커밋 해시>
# 커밋과 스테이징 취소(변경사항은 그대로)
```

### 2.3. --hard
```powershell
$ git reset --hard <커밋 해시>
# 커밋, 스테이징, 변경까지 취소
```

> ⚠️얘도 위험   
> 브랜치 관리 주의 / 리모트 리포지토리에서 하지 말 것

## 3. git revert
- 설정한 커밋 해시의 커밋을 되돌리는 내용을 Staging Area에 올림

#### 1.
```powershell
$ git revert <커밋 해시>
# 커밋 전으로 되돌리는 내용을 스테이징
```
#### 2.
```powershell
$ git revert --no-edit <커밋 해시>
# --no-edit 옵션: 편집기에 진입하지 않게 해준다.
```
> ✅   
> 가장 안전한 방법   
> 하지만 커밋 전에 실수를 먼저 방지하는게 중요