# 자주 만나는 문제

## 1) GitHub Pages가 404를 반환합니다
- Settings ▸ Pages ▸ Branch가 `gh-pages`로 설정되었는지 확인
- 배포 워크플로가 성공했는지 Actions 탭 확인

## 2) CI에서 `mkdocs build --strict` 실패
- `mkdocs.yml`의 `nav:` 경로/철자, 들여쓰기를 확인하세요(YAML 공백 중요)
- 참조된 페이지가 없는지, 링크가 깨지지 않았는지 점검

## 3) Vale가 규칙을 못 찾음
- `.vale.ini` 파일 경로 확인
- 커스텀 스타일은 `.vale/styles/...` 경로 아래 존재해야 합니다
- `vale sync`로 스타일 동기화(외부 스타일 사용 시)

## 4) markdownlint 오류가 너무 많음
- `.markdownlint.jsonc`에서 팀 규칙에 맞게 완화하거나 예외를 설정하세요
