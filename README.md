# DejaFix repo

DejaFix(장애 대응 코파일럿)를 파트별 별도 프로젝트로 나누어 문서화하는 저장소다. 원본 코드는 [DejaFix/DejaFix](https://github.com/DejaFix/DejaFix)에 있다.

## 구조

| 폴더 | 내용 |
|---|---|
| [`frontend/`](frontend/) | 화면 (React + Vite + TypeScript) |
| [`backend/`](backend/) | API·인증·채팅 중계·메일 워커 (FastAPI) |
| [`agent/`](agent/) | AI Agent: 분석·계획·채팅 답변 생성 |
| [`mcp/`](mcp/) | MCP 서버 모음 (mcp-zabbix 등) |
| [`docs/common/`](docs/common/) | 프론트엔드 공용 템플릿 문서 (토큰·컴포넌트·패턴·UI 규칙) |
| [`common-guidelines.md`](common-guidelines.md) | 공용 지침서: 모든 프로젝트가 따르는 규칙 |

## 읽는 순서

1. [`common-guidelines.md`](common-guidelines.md): 작업 기준, 안전 원칙, Git·PR, 계약 복사 규칙
2. 맡은 폴더의 `README.md`
3. 프론트엔드라면 [`docs/common/README.md`](docs/common/README.md)

## 규칙 요약

- 자기 폴더 밖 파일은 수정하지 않고 Issue로 요청한다.
- 계약 문서는 쓰는 폴더마다 복사하고, 원본은 한 곳에만 둔다. 복사본은 직접 고치지 않는다.
- 비밀값은 `.env`에만 두고 저장소에는 올리지 않는다.
- 상세 내용은 공용 지침서를 따른다.