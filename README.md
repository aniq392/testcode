# testcode
test code read me

test in pc 
Git에서 로그인하는 방법은 보통 두 가지입니다.

1. GitHub 계정 정보 설정
- 사용자 이름:
  - git config --global user.name "당신의 이름"
- 이메일:
  - git config --global user.email "your@email.com"

2. 원격 저장소에 로그인
- HTTPS 방식으로 연결할 때:
  - git push origin main
  - 그때 GitHub 아이디/비밀번호 또는 토큰을 입력합니다.
  - 최근에는 비밀번호 대신 Personal Access Token(PAT)을 사용합니다.

3. SSH 방식으로 인증
- SSH 키 생성:
  - ssh-keygen -t ed25519 -C "your@email.com"
- 키 확인:
  - cat ~/.ssh/id_ed25519.pub
- GitHub 설정에서 SSH keys에 붙여넣기
- 테스트:
  - ssh -T git@github.com

핵심 포인트
- Git 자체는 “로그인”보다 “인증”에 가깝습니다.
- HTTPS는 사용자명/토큰이 필요하고,
- SSH는 키 기반 인증입니다.

가장 많이 쓰는 방법
- HTTPS: git push 할 때 토큰 입력
- SSH: 한 번 설정해두면 편함

원하시면 다음으로:
- GitHub에 SSH로 연결하는 단계별 방법
- GitHub 토큰 만드는 방법
중 하나로 더 자세히 알려드릴게요.



