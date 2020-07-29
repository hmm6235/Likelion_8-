# github-practice

Git을 사용하기 위한 원격 저장소(repository)의 사용방법에 관한 것 입니다.
-----------------------------------------------------------------------------

1. Remote Repository를 생성
* Create a new repository
  * project명 설정
  * public / private 의 권한을 고려하여 선택

2. github에 올릴 소스코드 파일의 경로를 git bash를 이용하여 경로이동
  * cd(change directory)명령어를 이용하여 경로변경
  * pwd(print Working Directory)명령어를 이용하여 현재 어떤 디렉토리경로에 있는지 절대경로로 표시하여 현재 경로 파악

3. git bash console창에서 repository 연결

3-1. git init
> git 저장소를 초기화

3-2. git remote add origin repository address( 레포지토리 주소-> http:// )
> 로컬 저장소와 원격 저장소(remote repository) 를 연결

3-3. git add .
> index에 파일을 추가하는 명령
> 폴더에 변경된 모든파일 staging area에 올리기

3-4. git commit -m "원하는 내용"
> git commit -m "커밋 메시지"
>> 스테이징 영역의 파일들을 commit
>> -m은 커밋 메시지 옵션
>> 여러 줄의 커밋메시지는 여러개의 -m을 이용하여 처리 가능
>> 유사시 돌아갈 수 있는 저장소의 체크포인트 생성

3-5. git push origin master


--------------------------------------------------------------------------------
## Github에서 자주쓰는 명령어

1. git branch 브랜치 명
> 새로운 브랜치를 생성

2. git checkout 브랜치 명
> 해당 브랜치로 이동

3. git push origin 브랜치
> 원격 저장소의 특정 브랜치에 프로젝트 저장

4. git pull origin 브랜치
> 원격 저장소의 특정 브랜치에서 변경사항 pull 해오기

* push vs pull
push -> 올리겠다.
pull -> 다운해오겠다.

5. git clone http:// 원격저장소 주소.git
> 원격 저장소에 있는 파일 전체 복사 [ 자주 사용하는 명령어 ]

6. git status 
> git 저장소의 상태를 확인

---------------------------------------------------------------------------
## 다른 사람과 협업하기 위한 환경 생성하기

1. 원격 저장소 생성
2. 팀원을 Collaborator 로 추가
3. 초기 프로젝트 push
4. 팀원들의 로컬에 프로젝트 pull
5. 팀원 각자의 브랜치를 생성하여 작업
6. 브랜치에 작업한 내용을 push
7. Master와 merge 하기 전 pull request
8. Pull request 확인 후 Master과 merge

---------------------------------------------------------------------------
## 팀원과 Collaborator 로 추가되지 않았을 때, fork를 이용하여 협업

1. 작업 하고 싶은 Repository fork 해오기 [오른쪽 상단에 있는 fork 선택]
2. 자신의 로컬에서 작업
3. 변경사항을 자신의 브랜치에 push
4. 원본 레포지토리 소유자에게 Pull request 요청
5. 소유자가 pull request를 승인하여 merge 하면 자동으로 collaborator 추가



