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
> 로컬 저장소로 사용할 폴더를 생성하여 해당 폴더 이동

3-2. git remote add origin repository address(레포지토리 주소)

3-3. git add .
> index에 파일을 추가하는 명령

3-4. git commit -m "원하는 내용"
> git commit -m "커밋 메시지"
>> 스테이징 영역의 파일들을 commit
>> -m은 커밋 메시지 옵션
>> 여러 줄의 커밋메시지는 여러개의 -m을 이용하여 처리 가능

3-5. git push origin master


