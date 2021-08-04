# 기초 CLI 명령어

> CLI : Command Line Interface
>
> GUI 환경인 윈도우와는 다른 인터페이스를 지닌다.

* ls : 목록

  ```bash
  $ ls
  1.txt
  ```

* touch : 파일 만들기

  ```bash
  $ touch <파일명>
  $ touch README.md
  ```

* pwd : 현재 작업 디렉토리 출력 (print working directory)

  ```bash
  $ pwd
  /c/Users/lec/Desktop/실습1

* mkdir : 디렉토리 만들기 (make directory)

  ```bash
  $ mkdir test
  ```

* cd : 디렉토리 이동 (change directory)

  ```bash
  $ cd test
  ~/Desktop/실습1/test $ cd ..
  ~/Desktop/실습1 $ 
  ```

  * `..` : 상위 디렉토리
  * `.` : 현재 디렉토리

```bash
$ git status
On branch master
# 트래킹되고 있지 않은 파일들 (Working directory)
Untracked files:
# Staging area에 포함시키기 위해서는 git add를 해.
# Staging area -> 커밋 대상 파일들 모아놓는 공간(커밋이 될 예정인 것들)
  (use "git add <file>..." to include in what will be committed)
        new.txt

# 커밋하기 위해 추가된 것은 없는데,untracked files는 존재한다.
# Working directory -> 파일 있어
# Staging area -> 파일 없어
nothing added to commit but untracked files present (use "git add" to track)
```

```bash
$ git status
On branch master
# 커밋될 변경사항들 (staging area)
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.txt
```

```bash
$ git status
On branch master
# Staging area (Staged O)
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.txt


# staged X (커밋을 위해)
# Working directory
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   2.txt

# 트래킹 X
# Working directory
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hi.txt


```



## 요약 및 추가 용어 정리

* __ls__ : list의 약자. 목록 보여줘
* touch : 파일 생성. touch 만들파일명.확장자 bash 환경에 쓰는 명령어가 아니기 때문에 앞에 git 안붙음. 리눅스 공통.
* __pwd__: print working directory. 현재 폴더 위치 알려줘
* __mkdir test__: make directory. 디렉토리 생성.
* __cd test__: change directory. 경로 바꿈
* __git reset__: 삭제
* __git clone 주소명__: 복사하기



### 원격저장소에 올리는 과정

* 저장소 만들기
  * git init
* 작업하면서 버전 기록하기
  * git add 파일명
  * git commit -m '버전구분하기 위한 메시지'
* 상태 확인
  * git log
  * git status
* 원격저장소
  * git remote add origin 주소(url) => 깃아….원격저장소(remote) 추가해줘 .(add) origin 이라는 이름으로. origin이 url 대신 붙이는 이름.
  * git push origin master



> 너무......어렵다......복잡하다.......하지만........난...할수있다^^...!

