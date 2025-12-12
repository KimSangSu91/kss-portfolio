# 포트폴리오 웹사이트

김상수의 포트폴리오 웹사이트입니다.

## GitHub Pages 배포 방법

### 1. GitHub 저장소 생성
1. GitHub에 로그인 후 https://github.com/new 에서 새 저장소 생성
2. 저장소 이름: `kss-portfolio` (또는 원하는 이름)
3. Public으로 설정
4. README, .gitignore, license는 추가하지 않음 (이미 있음)

### 2. 로컬에서 Git 초기화 및 푸시

프로젝트 디렉토리에서 다음 명령어를 실행하세요:

```bash
# Git 초기화 (이미 되어있다면 생략)
git init

# 모든 파일 추가
git add .

# 첫 커밋
git commit -m "Initial commit: Portfolio website"

# GitHub 저장소 연결 (저장소 URL을 실제 URL로 변경)
git remote add origin https://github.com/KimSangSu91/kss-portfolio.git

# 메인 브랜치로 푸시
git branch -M main
git push -u origin main
```

### 3. GitHub Pages 활성화

1. GitHub 저장소 페이지로 이동
2. Settings 탭 클릭
3. 왼쪽 메뉴에서 Pages 클릭
4. Source에서 "Deploy from a branch" 선택
5. Branch를 `main`으로, 폴더를 `/ (root)`로 설정
6. Save 클릭

### 4. 웹사이트 접속

몇 분 후 다음 URL로 접속 가능합니다:
- `https://kimSangSu91.github.io/kss-portfolio/`

또는 저장소 이름을 `username.github.io` 형식으로 만들었다면:
- `https://kimSangSu91.github.io/`

## 파일 구조

```
kss-portfolio/
├── index.html          # 메인 페이지
├── project-01.html     # 프로젝트 1 상세 페이지
├── project-02.html     # 프로젝트 2 상세 페이지
├── project-sub.html   # 기타 프로젝트 페이지
├── style.css          # 스타일시트
├── images/            # 이미지 파일들
└── README.md          # 이 파일
```

## 로컬에서 테스트

브라우저에서 `index.html` 파일을 직접 열거나, Live Server 확장 프로그램을 사용하여 테스트할 수 있습니다.

