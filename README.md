# VS Code LaTeX 작업 환경

이 폴더는 **VS Code + LaTeX Workshop + TeX Live 2026 + latexmk** 조합으로
설정되어 있습니다. 기본 엔진은 한글과 유니코드를 편하게 다루는 LuaLaTeX입니다.

## 사용법

1. VS Code에서 `main.tex`를 엽니다.
2. 최초 한 번 `Ctrl+Alt+B`로 빌드합니다.
3. `Ctrl+Alt+V`를 누르면 PDF가 오른쪽 편집기 그룹에 열립니다.
4. 이후에는 입력을 멈춘 지 약 0.8초 뒤 자동 저장·빌드되고 PDF도 자동 갱신됩니다.

완성된 PDF는 `output/pdf/main.pdf`입니다. LaTeX 빌드 결과가 이미 PDF이므로 별도
내보내기 과정 없이 이 파일을 그대로 사용하면 됩니다.

## 자주 쓰는 단축키

- `Ctrl+Alt+B`: PDF 빌드
- `Ctrl+Alt+V`: 오른쪽에 PDF 열기
- `Ctrl+Alt+J`: 현재 소스 위치를 PDF에서 찾기
- PDF에서 더블 클릭: 해당 위치의 LaTeX 소스로 이동
- `Ctrl+Alt+C`: 보조 빌드 파일 정리

영문 전용 문서처럼 pdfLaTeX가 필요한 경우 명령 팔레트의
`LaTeX Workshop: Build with recipe`에서 `latexmk (pdfLaTeX · TeX Live 2026)`을
선택할 수 있습니다.
