# Docs-as-Code Starter (MkDocs + Material + Vale + Markdownlint)

이 리포는 `docs-as-code` 파이프라인의 최소 템플릿입니다.

## 빠른 시작
```bash
# 1) 가상환경(선택)
python -m venv .venv && . ./.venv/bin/activate  # macOS/Linux
# Windows PowerShell:  .\.venv\Scripts\Activate.ps1

# 2) MkDocs(Material) 설치
pip install mkdocs mkdocs-material

# 3) 로컬 미리보기
mkdocs serve -a 0.0.0.0:8000
# 브라우저에서 http://localhost:8000 접속
```

## Lint (선택 사항)
- Vale 설치: macOS `brew install vale` / Windows(winget) `winget install Vale.Vale`
- 마크다운 린트: `npm i -D markdownlint-cli2` → `npm run lint:md`

## 배포(GitHub Pages)
1. GitHub 저장소 만들고 소스 푸시
2. Actions 탭에서 워크플로 허용
3. Settings ▸ Pages ▸ Branch를 `gh-pages`로 설정

자세한 튜토리얼은 `docs/how-to/hello-tutorial.md`를 참고하세요.
