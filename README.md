# Github메모


github 토큰

#####

github id

jaemin.ko98@gmail.com

kkojam98@gmail.com

## Github 버전 관리


**커밋 Commit :**

Git에 파일을 추가하거나 변경 내용을 저장

**푸시 Push :**

Github(또는 원격 저장소)에 파일을 추가하거나 변경 내용을 저장

**풀 Pull :**

Github(또는 원격 저장소)에서 파일을 다운로드하는 작업

## git command


git init

: 로컬 폴더를 깃 저장소로 설정 및 초기화

git status

: working directory와 staging area의 상태를 확인

git add

: 다음 커밋을 기록할 때까지 변경분을 모아놓음

옵션

- add .
디렉토리의 모든 변경내용을 스테이징 영역으로 넘김
- add -A
작업 디렉토리 내의 변경내용을 모두 넘김
- add “file name”
해당 파일만 넘김

git commit

: 스테이징 상태의 파일들을 저장소로 옮김

옵션

- -m “커밋메세지”
메세지와 함께 커밋

git push
: 마지막으로 커밋한 사항을 git repository에 올림

- git push origin main을 이용하여 해당 리포지토리에 업로드

git remote -v
: 현재 연결된 github 리포지토리 확인

git clone <링크>

: 리포지토리를 링크에서 가져옴, 자동연동

## ./gitignore


git add에 파일을 포함시키고 싶지 않은 경우, 업로드를 무시할 파일을 설정할 수 있음

## 새로운 리포지토리 추가


github에서 새로운 리포지토리 생성

이후 git clone <리포지토리 링크>

## pull and merge


로컬 저장소와 원격저장소의 내용이 다를시 pull을 통해 변경사항을 받아오고 merge시킴

- git fetch origin
: 원격저장소의 내용을 로컬저장소로 가져오고 임시로 FETCH_HEAD라는 이름의 브랜치를 생성( git checkout FETCH_HEAD명령으로 원격저장소에서 가져온 업데이트를 확인할 수 있음)
- git merge origin/main
: merge로 가져온 내용을 main 브랜치에 merge함, 만약 충돌이 발생했을 시 직접 파일을 수정해 줘야 한다.
- git pull origin main
: fetch와 merge를 한번에 진행하는 명령어
- git config pull.rebase false
: ??
- git pull origin main
: 원격저장소 내용을 merge시킴
- `git push -u origin +master`

 “+”옵션을 사용하여 강제 push
![Untitled](/Github메모%201fed820c4ad54549bd3298053a3f133a/Untitled.png)

## .gitignore 생성 사이트


[gitignore.io](https://www.toptal.com/developers/gitignore)
