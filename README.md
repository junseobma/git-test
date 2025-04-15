# Git 사용법 정리

이 레포지토리는 코딩애플의 [**Git & GitHub 강의**](https://codingapple.com/course/git-and-github/)를 바탕으로 작성되었습니다.

Git의 주요 명령어를 실습하며 정리한 학습용 자료입니다.  
각 `.txt` 파일은 특정 Git 기능 또는 명령어를 다루고 있습니다.  

---

## 파일 목록 및 내용 요약

| 파일 이름       | 내용 요약 |
|----------------|-----------|
| `git.txt`      | Git의 기본적인 명령어 사용법 예시 |
| `git2.txt`     | 로컬 저장소 설정, 커밋 및 상태 확인 |
| `git3.txt`     | 원격 저장소 연결 및 푸시(push) 과정 |
| `branch.txt`   | 브랜치 생성, 전환, 삭제 관련 명령어 |
| `merge.txt`    | 브랜치 병합 (merge) 과정 실습 |
| `stash.txt`    | 변경사항 임시 저장(stash) 사용법 |
| `restore.txt`  | 파일 변경 취소 (`git restore`) 사용 예시 |
| `test0.txt` ~ `test4.txt` | 브랜치 실습, 충돌 테스트 등을 위한 예제 파일 |

---

## 주요 Git 명령어 요약

### 저장소 초기화 및 설정
```bash
git init
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

### 파일 추가 및 커밋
```bash
git add .
git commit -m "커밋 메시지"
```

### 원격 저장소 연결 및 푸시
```bash
git remote add origin https://github.com/yourusername/repo-name.git
git push -u origin main
```

### 브랜치 작업
```bash
git branch 브랜치이름       # 새 브랜치 생성
git checkout 브랜치이름     # 브랜치 전환
git merge 브랜치이름        # 브랜치 병합
```

### 변경사항 임시 저장 (stash)
```bash
git stash             # 변경사항 임시 저장
git stash list        # 저장 목록 확인
git stash pop         # 가장 최근 stash 복원
```

### 변경 취소 및 복원
```bash
git restore 파일명           # 변경 취소
git restore --staged 파일명  # staging에서 취소
```

---

## 참고 자료
> [Git 공식 문서](https://git-scm.com/doc)  
> [GitHub Docs](https://docs.github.com/)
