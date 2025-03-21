## **1️⃣ Git을 처음 설정하는 방법**

💡 **처음 한 번만 진행하면 됩니다.**

### ✅ **Git 다운로드 (없다면 설치)**

1. [Git 공식 사이트](https://git-scm.com/)에서 다운로드 후 설치
2. 설치 완료 후 **Git Bash** 또는 **CMD(명령 프롬프트)** 실행

### ✅ **Git 저장소 클론(복사)하기**

1️⃣ **CMD 또는 Git Bash 실행**

- `윈도우 + R` → `cmd` 입력 후 Enter

2️⃣ **드라이브로 이동**

예시) `E:`

3️⃣ **예시) 옵시디언 폴더로 이동 (없다면 생성 후 이동)**

`mkdir 예시)옵시디언 cd 예시)옵시디언`

4️⃣ **GitHub에서 저장소 가져오기 (복사)**

`git clone https://github.com/Blacktailz2188/Lagvar.git cd Lagvar`

✅ **이렇게 하면 `.git` 폴더가 자동 생성되면서 네 저장소와 동기화됨!**  
✅ **이제 Obsidian을 실행하면 Git 플러그인이 자동으로 감지하고 연동됩니다.**





### 1. Git 사용자 정보 설정

터미널에서 다음 명령어를 사용하여 사용자 이름과 이메일 주소를 설정합니다:

bash

Copy

git config --global user.name "당신의 이름"
git config --global user.email "당신의 이메일 주소"

예를 들어:

bash

Copy

git config --global user.name "John Doe"
git config --global user.email "johndoe@example.com"

### 2. 설정 확인

설정이 제대로 되었는지 확인하려면 다음 명령어를 사용합니다:

bash

Copy

git config --global user.name
git config --global user.email

### 3. 저장소별 설정 (선택 사항)

특정 저장소에 대해 다른 사용자 정보를 설정하려면, 해당 저장소 디렉토리에서 `--global` 옵션 없이 명령어를 실행합니다:

bash

Copy

git config user.name "저장소별 이름"
git config user.email "저장소별 이메일"

### 4. SSH 키 설정 (선택 사항)

SSH를 사용하여 원격 저장소에 접근하는 경우, SSH 키가 제대로 설정되었는지 확인합니다. SSH 키를 생성하고 원격 저장소에 추가하는 방법은 다음과 같습니다:

1. SSH 키 생성:
    
    bash
    
    Copy
    
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    
2. 생성된 공개 키를 복사:
    
    bash
    
    Copy
    
    cat ~/.ssh/id_rsa.pub
    
3. 복사한 공개 키를 GitHub, GitLab 등의 원격 저장소 설정에 추가합니다.
    

### 5. 권한 확인

원격 저장소에 접근 권한이 있는지 확인합니다. 저장소 소유자나 관리자에게 접근 권한을 요청해야 할 수도 있습니다.

이 단계들을 따르면 "당신이 누군인지 모른다"는 메시지가 해결될 것입니다. 추가로 궁금한 점이 있으면 언제든지 물어보세요!