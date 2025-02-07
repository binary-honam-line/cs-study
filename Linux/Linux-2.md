# 👽**18 Most-used Linux Commands You Should Know**

## 🗣️리눅스 명령어

- 리눅스 명령어는 운영체제 **상호 작용**하기 위한 지시어(instructions)이다.
- 파일/디렉터리 관리, 시스템 프로세스 제어, 네트워크 설정와 같은 작업을 수행할 수 있다.

## 📔자주 사용되는 리눅스 명령어

### 📂 **파일 및 디렉터리 관리 명령어**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `ls` | 현재 디렉터리의 파일 및 폴더 목록을 출력 | `ls -l` (자세한 정보 포함) |
| `cd` | 디렉터리 이동 | `cd /home/user` |
| `mkdir` | 새로운 디렉터리 생성 | `mkdir new_folder` |
| `rm` | 파일 또는 디렉터리 삭제 | `rm file.txt`, `rm -r folder` |
| `cp` | 파일 및 디렉터리 복사 | `cp file1.txt file2.txt`, `cp -r dir1 dir2` |
| `mv` | 파일 및 디렉터리 이동 또는 이름 변경 | `mv old.txt new.txt` |

---

### 🔍 **파일 및 문자열 검색**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `grep` | 특정 패턴을 포함하는 문자열 검색 | `grep "hello" file.txt` |
| `find` | 특정 조건에 맞는 파일 및 디렉터리 검색 | `find /home -name "*.txt"` |

✔ **특정 파일 내용 검색**

```bash
grep "error" /var/log/syslog
# var/log/syslog 에서 "error"라는 단어가 포함된 줄을 검색

```

✔ **특정 파일 찾기**

```bash
find /home -type f -name "document.txt"
# 홈 디렉터리(/home)에서 document.txt라는 이름의 파일을 찾는 명령어
# -type f : 파일만 검색 + 디렉터리는 제외

find /var/log -type f -name "*.log"
# /var/log 디렉터리에서 .log 확장자를 가진 모든 파일 찾기

```

---

### 📦 **압축 및 아카이브**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `tar` | tar 압축 파일을 생성 또는 해제 | `tar -cvf archive.tar folder/` |

✔ **압축 파일 생성**

```bash
tar -czvf archive.tar.gz folder/

```

✔ **압축 해제**

```bash
tar -xzvf archive.tar.gz

```

---

### 📝 **텍스트 파일 보기 및 편집**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `cat` | 파일 내용 출력 | `cat file.txt` |
| `vi` | `vi` 텍스트 편집기 실행 | `vi file.txt` |

✔ **파일 내용 출력**

```bash
cat /etc/passwd

```

✔ **vi 편집기 사용**

```bash
vi file.txt
# i : 입력 모드 진입
# ESC + :wq : 저장 후 종료

```
> ※ vim, vi 차이점
>  vim = Vi Improved -> vi 확장버전이 vim 이다.

---

### 📊 **프로세스 및 리소스 관리**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `top` | 현재 실행 중인 프로세스 및 시스템 리소스 확인 | `top` |
| `ps` | 현재 실행 중인 프로세스 목록 표시 | `ps aux` |
| `kill` | 특정 프로세스 종료 | `kill 1234` |

✔ **프로세스 확인**

```bash
ps aux | grep apache

```

✔ **프로세스 종료**

```bash
kill -9 1234
# -9 : kill 옵션 중 하나. 강제 종료 + 저장 작업 없이 즉시 종료된다.
# -15 : default 종료 요청 + 종료 작업 수행 후 종료

```

✔ **실시간 프로세스 모니터링**

```bash
top

```

---

### 💾 **디스크 공간 확인**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `df` | 디스크 사용량 확인 | `df -h` |
| `du` | 특정 파일 및 디렉터리의 공간 사용량 확인 | `du -sh folder/` |

✔ **디스크 사용량 보기**

```bash
df -h

#Filesystem      Size  Used Avail Use% Mounted on
#/dev/root       6.8G  2.4G  4.4G  36% /
#tmpfs           479M     0  479M   0% /dev/shm
#tmpfs           192M  892K  191M   1% /run

```

✔ **디렉터리별 사용량 보기**

```bash
du sh -back
# 17M     back/

```

---

### 🌐 **네트워크 관리 및 테스트**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `ifconfig` | 네트워크 인터페이스 설정 및 확인 | `ifconfig eth0` |
| `ping` | 네트워크 연결 상태 확인 | `ping google.com` |

✔ **네트워크 인터페이스 확인**

```bash
ifconfig

```

✔ **서버 응답 확인**

```bash
ping google.com

```

---

### 🔐 **파일 권한 및 소유권 관리**

| 명령어 | 설명 | 사용 예시 |
| --- | --- | --- |
| `chmod` | 파일 및 디렉터리의 권한 변경 | `chmod 755 script.sh` |
| `chown` | 파일 및 디렉터리의 소유권 변경 | `chown user:user file.txt` |

✔ **권한 변경 예시**

```bash
chmod u+x script.sh  # 사용자에게 실행 권한 추가
chmod 644 file.txt    # 소유자는 읽기/쓰기, 다른 사용자는 읽기만 가능

```

written by semi