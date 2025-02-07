# GIT
## 깃 명령어들이 어떻게 작동하는가
우선, 코드가 저장된 위치를 파악하는 것이 중요합니다. 

일반적으로 저장 위치는 2가지가 있는데, 하나는 Github 원격저장소에 있고, 다른 하나는 로컬 컴퓨터에 있습니다.

하지만,이것은 정확하지는 않습니다. 

Git은 3가지 로컬 저장소를 관리하고 있으므로, 코드는 4곳에서 관리 하고 있음을 말합니다.

![alt text](git-commands.png)

작업 디렉토리: 파일을 편집하는 위치

스테이징 영역: 다음 커밋을 위해 파일을 보관하는 임시 위치

로컬 저장소: 커밋된 코드가 포함되어 있습니다

원격 저장소: 코드를 저장하는 원격 서버

대부분의 Git 명령어는 주로 이 4 위치 사이에서 파일을 이동합니다.

## 명령어
### 깃 정보 설정
git config —global user.name “사용자이름 설정” 이름 설정

git config —global user.email “사용자 이메일” 이메일 설정

git config — list  설정된 정보 확인



git init  폴더에 깃을 추가하여 버전관리를 하겠다!

git remote add origin https://github.com/binary-honam-line/cs-study.git 원격 저장소 연결

git remote -v 원격 저장소 확인

git add <file> 깃에 파일을 추가하겠다!

git commit -m “message” 깃에 등록하겠다! 메시지 추가

git status 저장소의 상태 확인하겠다! (스테이지에 올라가있는 파일 확인)

git log 커밋을 확인 할 수있다.



git clone https://github.com/keen1014/qwhfquiwehfldcas.wqefshf? 내용을 복제한다.

git push  remote repository로 보낸다.

git pull remote repository에 있는 내용을 가져온다.

git fetch remote repositiory에서 변경 내용을 가져온다.
