# git

## 기초 CLI 명령어

> CLI :
>
> GUI : 

* ls: 목록

* touch: 파일 만들기

  ```bash
  $ touch <파일명>
  $ touch README.md
  ```

  

* pwd: 현재 작업 디렉토리 출력

  ```bash
  $ pwd
  ```

  

* mkdir test: 디렉토리 만드는 것

* cd: 폴더이동

  * change directory
    `.. `: 상위폴더
    `. `: 현재 디렉토리

## 기본 명령어

### $ git init

특정 폴더를 git 저장소(repository)를 만들어 git으로 관리

* .git 폴더가 생성되며
* git bash에서는 (master)라는 표기 확인가능

### $ git add <file>

* working directory 상의 변경내용을 staging area에 추가하기 위해 사용
  * untracked 상태의 파일을 staged로 변경
  * modified 상태의 파일을 staged로 변경

### 파일 라이프 사이클

* Working directory의 모든 파일은 특정상태를 가지며, git 명령어를 통해 변경
  * Tracked: 이전부터 버전으로 관리되고 있는 파일
    * Unmodified: git status에 나타나지 않음
    * Modified
    * Staged
  * Untracked: 버전으로 관리된 적 없는 파일(파일을 새로 만든 경우)

### git commit

* staged 상태의 파일들을 커밋을 통해 버전으로 기록
* SHA-1 해시를 사용하여 40자 길이의 체크섬을 생성하고, 이를 통해 고유한 커밋을 표기

## git log

* 현재 저장소에 기록된 커밋을 조회
* 다양한 옵션을 통해 로그를 조회할 수 있음

