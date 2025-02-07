# 📁Linux File Systems

## 📌**개요**

리눅스 파일 시스템은 마치 사람들이 원하는 곳에 집을 지어 놓은 무질서한 마을과 같았다. 

그러나 1994년, 파일 시스템 계층 표준,**FHS (**Filesystem Hierarchy Standard)이 도입되면서 리눅스 파일 시스템에 질서를 부여하게 되었다.

## 📁FHS (Filesystem Hierarchy Standard)

- **파일 시스템 계층구조 표준으로,**  리눅스의 주 디렉토리를 정의한다.
- FHS와 같은 표준을 적용함으로써 소프트웨어는 다양한 리눅스 배포판에서 일관된 파일 구조를 유지할 수 있다.
- 모든 리눅스 배포판이 이 표준을 엄격하게 따르는 것은 아니다. 각 배포판은 고유한 요소를 추가하거나 특정 요구 사항에 맞춰 조정되기도 한다.

## 🐧리눅스 파일 시스템 구조 정리
![image](https://github.com/user-attachments/assets/4108f348-5af8-407b-a828-7b4a5193e3b6)

1. **/bin** 
    - essential command binaries
    - **필수 기본 명령어가 포함된 디렉터리**
    - ex)
        - `/bin/ls` (디렉터리 목록 출력)
        - `/bin/cp` (파일 복사)
        - `/bin/mv` (파일 이동)
        - `/bin/rm` (파일 삭제)
        
2. **/boot**
    - system boot loader files
    - 시스템 부팅에 필요한 **부트 로더(boot loader) 및 커널 파일**이 저장된 디렉터리
    - ex)
        - `/boot/vmlinuz` (커널 이미지 파일) → 이 파일을 메모리에 로드하고 실행
        - `/boot/grub/` (GRUB 부트 로더 설정 파일)
        
3. **/dev**
    - device files
    - **하드웨어 장치**를 파일 형태로 저장한 디렉터리 (ex. 디스크, 키보드, 마우스 etc)
    - ex)
        - `/dev/sda` (하드 디스크 장치)
        - `/dev/null` (모든 데이터를 버리는 장치)
        - `/dev/tty` (터미널 장치)
        
4. **/etc**
    - Host-specific system-wide configuration files
    - **설정 파일**이 저장된 디렉터리. 모든 사용자가 공유한다.
    - ex)
        - `/etc/passwd` (사용자 계정 정보)
        - `/etc/hosts` (호스트네임 설정)
        - `/etc/fstab` (파일 시스템 마운트 정보)
        
5. **/home**
    - User home directory
    - 일반 사용자 계정마다 할당되는 **개인 디렉터리**
    - 각 사용자는 `/home/사용자명` 경로를 가지며, 개인 파일과 설정을 저장
    - ex)
        - `/home/user1` (user1의 홈 디렉터리)
        - `/home/user2` (user2의 홈 디렉터리)
        
6. **/media**
    - Media file such as CD-ROM
    - **이동식 저장 장치**(mounted devices)를 자동으로 연결하는 디렉터리 (ex. CD-ROM. USB)
    - USB, CD를 삽입하면 /media 하위 디렉터리에 마운트된다.
    
7. **/mnt**
    - Temporary mounted filesystems
    - 임시로 다른 파일 시스템을 마운트할 때 사용하는 디렉터리
    
8. **/opt**
    - Add-on application software packages
    - 기본 패키지 관리자(예: `apt`, `yum`)가 아닌 **별도로 설치한 소프트웨어**가 저장되는 디렉터리
    - 수동으로 설치한 프로그램이 저장
    
9. **/proc**
    - Automatically generated file system
    - 시스템의 **커널과 프로세스 정보**를 제공하는 가상 파일 시스템
    - ex)
        - `/proc/cpuinfo` (CPU 정보)
        - `/proc/meminfo` (메모리 사용량)
        - `/proc/uptime` (시스템 부팅 시간)
        
10. **/root**
    - Home directory for root user
    - `root`(관리자)의 개인 디렉터리 → like /home
    
11. **/run**
    - Run-time program data
    - 시스템이 실행되는 동안 필요한 **일시적인(run-time) 데이터**가 저장
    
12. **/sbin**
    - System binaries
    - 시스템 관리자가 사용하는 **관리자용 명령어**(system binaries)가 포함된 디렉터리
    - 일반 사용자는 실행할 수 없으며, **루트 사용자**만 실행할 수 있다.
    - ex)
        - `/sbin/shutdown` (시스템 종료)
        - `/sbin/fsck` (파일 시스템 검사)
        - `/sbin/mount` (파일 시스템 마운트)
        
13. **/srv**
    - Site-specific data served by this system
    - 웹 서버, FTP 서버와 같은 **서비스 관련 데이터**가 저장되는 디렉터리
    - ex)
        - `/srv/www` (웹 서버 데이터)
        - `/srv/ftp` (FTP 서버 데이터)
        
14. **/sys**
    - Virtual directory providing information about the system
    - **하드웨어 및 커널 관련 정보**를 제공하는 가상 디렉터리
    - `/proc`과 유사하지만, 더 **하드웨어 중심적인 정보**를 제공
15. **/tmp**
    - Temporary files
    - 프로그램이 생성하는 **임시 파일**을 저장하는 디렉터리
    - 재부팅 하면 내용이 자동으로 삭제된다.
16. **/usr**
    - Read-only user files
    - 시스템의 **애플리케이션, 라이브러리, 문서**가 저장되는 디렉터리
17. **/var**
    - File that is expected to continuously change
    - 시스템이 운영되면서 **변하는 데이터를 저장**하는 디렉터리
    - ex)
        - `/var/log` (로그 파일)
        - `/var/tmp` (임시 데이터)
        - `/var/mail` (메일 데이터)

## ✏️정리

### 🖥 **필수 시스템 디렉터리**

이 디렉터리들은 리눅스 시스템이 부팅되고 정상적으로 작동하는 데 필수적이다.

| 디렉터리 | 설명 |
| --- | --- |
| `/` (루트) | 모든 파일과 디렉터리의 최상위 디렉터리 |
| `/bin` | 기본적인 실행 파일(일반 사용자 및 관리자 명령어) |
| `/sbin` | 시스템 관리 명령어 (관리자(root)만 실행 가능) |
| `/lib`, `/lib64` | 시스템 실행에 필수적인 라이브러리 파일 |
| `/boot` | 부팅 관련 파일 (커널, 부트로더 등) |
| `/dev` | 장치 파일 (하드디스크, USB, 터미널 등) |
| `/etc` | 시스템 설정 파일 (모든 사용자 및 서비스 설정 포함) |
| `/proc` | 가상 파일 시스템 (커널 및 프로세스 정보) |
| `/sys` | 하드웨어 정보 및 시스템 관련 파일 |

### 📂 **사용자 및 데이터 관련 디렉터리**

이 디렉터리들은 주로 사용자 데이터와 애플리케이션 실행 파일을 저장하는 역할을 한다.

| 디렉터리 | 설명 |
| --- | --- |
| `/home` | 일반 사용자 홈 디렉터리 (`/home/사용자명`) |
| `/root` | 루트 사용자의 홈 디렉터리 |
| `/usr` | 시스템 애플리케이션 및 라이브러리 (`/usr/bin`, `/usr/lib`) |
| `/opt` | 추가적으로 설치된 소프트웨어 패키지 |

### 📁 **변경이 많은 데이터 저장 디렉터리**

이 디렉터리들은 시스템 운영 중 **자주 변경되는 데이터**를 저장한다.

| 디렉터리 | 설명 |
| --- | --- |
| `/var` | 지속적으로 변경되는 데이터 (로그, 캐시, 메일 등) |
| `/var/log` | 시스템 로그 파일 저장 |
| `/var/tmp` | 임시 데이터 저장, 재부팅 시 삭제되지 않음 |
| `/tmp` | 임시 파일 저장소 (재부팅 시 삭제됨) |

### 📦 **마운트 및 외부 장치 관련 디렉터리**

이 디렉터리들은 외부 장치나 네트워크 드라이브를 연결할 때 사용된다.

| 디렉터리 | 설명 |
| --- | --- |
| `/media` | 자동으로 마운트되는 미디어 장치 (CD-ROM, USB 등) |
| `/mnt` | 수동으로 마운트하는 파일 시스템 (외장 하드 등) |
