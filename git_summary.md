
# Git 기본 흐름 요약

## 1. 초기화
```bash
git init
```
> 현재 폴더를 Git 저장소로 초기화합니다.

## 2. 파일 추가
```bash
git add 파일명      # 특정 파일 추가
git add .           # 모든 변경된 파일 추가
```
> 스테이징 영역에 파일을 올립니다.

## 3. 커밋
```bash
git commit -m "메시지"
```
> 변경사항을 로컬 저장소에 저장합니다.

## 4. 원격 저장소 연결
```bash
git remote add origin 원격주소
```
> GitHub 등 원격 저장소와 연결합니다.

## 5. 푸시
```bash
git push -u origin main
```
> 로컬 변경사항을 원격 저장소에 업로드합니다.

---

## 상태 확인 명령어
```bash
git status         # 현재 상태 확인
git log            # 커밋 히스토리 보기
git branch         # 현재 브랜치 확인
git checkout 브랜치명  # 브랜치 전환
```

---

## 전체 예시
```bash
echo "# 프로젝트명" > README.md
git init
git add .
git commit -m "초기 커밋"
git branch -M main
git remote add origin https://github.com/사용자명/저장소명.git
git push -u origin main
```
