# GitHub

### cd : change directory

- cd . : 현재 작업하고 있는 폴더
- cd .. : 상위폴더
- cd ~ : 홈디렉토리



### ls : list segments

- 현재 작업 디렉토리의 폴더 /파일 목록을 출력



### mkdir : make directory

- mkdir : make directory
- mkdir 'new folder2' : ' '붙이면 띄어쓰기 있는 폴더 이름명 가능



### mv / rm
- mv (파일명) [옮길 폴더]
- rm : 파일 삭제



## 유용한 단축키

 - 위, 아래 방향키 : 과거에 작성했던 기록 보여줌
 - tab : 폴더/파일 이름 자동 완성
 - ctrl + a : 커서가 맨 앞으로 이동
 - ctrl + e : 커서가 맨 뒤로 이동
 - ctrl + w : 커서가 앞 단어를 삭제
 - ctrl + l :  터미널 화면을 깨끗하게 청소(스크롤 올리면 과거 내역 조회 가능)
 - ctrl + insert : 복사
 - shift + insert : 붙여넣기



+ 파이썬 언어를 개발하기 위한 개발 환경
	+ vsCode 
	+ 파이참

# git
### 커밋기록자들 등록
 - git config --global -l : 이름, 이메일 확인

 - working directory : 로컬의 사용자 작업이 일어나는 곳
 - staging area : 커밋을 위한 파일 및 폴더가 추가되는 곳
 - repository(commits) : 변경사항(커밋)을 저장하는 곳

## git
#### git init
local directory 를 git으로 관리한다고 정의

#### git status
git 상태표시
 - untracked : git이 관리하지 않는 파일
 - tracked : git 이 관리하는 파일

#### git add(staging)
 - git add 파일이름(폴더이름)
 - git add. -> 전체 다

#### git commit
 - git commit -m "메시지"

#### git log(commit log)
 - --oneline : 한 줄로 축약해서 보여줍니다.
 - --graph : 브랜치와 머지 내역을 보여줍니다.
 - --all : 현재 브랜치를 포함한 모든 브랜치의 내역을 보여줍니다.
 - --reverse : 커밋 내역의 순서를 반대로 보여줍니다.(최신이 가장 아래)
 - -p : 파일의 변경 내용도 같이 보여줍니다.
 - -2 : 원하는 갯수 만큼의 내역을 보여줍니다. (2 말고 임의의 숫자 사용 가능)

## 원격 저장소 등록
 - git remote add <이름><주소>
*보통 remote 연결이 한개인 경우 origin을 사용함.
(git remote add origin https://github.com/bonfire8/gitpractice.git)*
 - git remote -v : repository 확인
 - git remote rm <이름> : 삭제

 + git push origin mastser : github에 올리기

#### github에 수정하는 과정
 - git add . /git add 파일이름
 - git commit -m " "
 - git push origin master
