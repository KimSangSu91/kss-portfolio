# GitHub Pages 배포 문제 해결 가이드

## 404 에러 해결 방법

### 1. 저장소 이름과 URL 확인
- GitHub 사용자명: `KimSangSu91`
- 저장소 이름: `kss-portfolio`
- 올바른 URL: `https://KimSangSu91.github.io/kss-portfolio/`

**주의**: GitHub Pages URL은 대소문자를 구분합니다!

### 2. GitHub Pages 설정 확인
1. 저장소 페이지로 이동
2. **Settings** 탭 클릭
3. 왼쪽 메뉴에서 **Pages** 클릭
4. **Source** 섹션 확인:
   - "Deploy from a branch" 선택
   - Branch: `main` (또는 `master`)
   - Folder: `/ (root)`
5. **Save** 클릭

### 3. 배포 상태 확인
1. 저장소 페이지에서 **Actions** 탭 클릭
2. "pages build and deployment" 워크플로우 확인
3. 배포가 진행 중이면 완료될 때까지 대기 (보통 1-2분)

### 4. 저장소 공개 설정 확인
- 저장소가 **Public**으로 설정되어 있어야 합니다
- Private 저장소는 GitHub Pro가 필요합니다

### 5. 브랜치 이름 확인
```bash
# 현재 브랜치 확인
git branch

# main 브랜치가 없다면 생성
git branch -M main
git push -u origin main
```

### 6. 파일이 올바르게 푸시되었는지 확인
```bash
# 원격 저장소의 파일 목록 확인
git ls-tree -r main --name-only
```

### 7. 캐시 문제
- 브라우저 캐시를 지우고 다시 시도
- 시크릿 모드에서 접속 시도
- 다른 브라우저에서 시도

## 일반적인 문제들

### 문제: "404 Not Found"
**해결책**:
- 저장소 이름과 사용자명의 대소문자 확인
- GitHub Pages 설정이 올바른지 확인
- 배포가 완료되었는지 Actions 탭에서 확인

### 문제: "Repository not found"
**해결책**:
- 저장소가 Public인지 확인
- 저장소 이름이 정확한지 확인

### 문제: 빈 페이지가 표시됨
**해결책**:
- `index.html` 파일이 루트 디렉토리에 있는지 확인
- 파일 경로가 올바른지 확인

## 올바른 배포 확인 방법

1. 저장소 → Settings → Pages
2. "Your site is live at" 메시지 확인
3. 표시된 URL이 정확한지 확인

## 추가 도움말
- GitHub Pages 문서: https://docs.github.com/en/pages
- 문제가 계속되면 GitHub Support에 문의

