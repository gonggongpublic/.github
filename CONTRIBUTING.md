# 공공팀 협업 규칙

WBS의 말단 작업 하나에 이슈 하나를 만들고, 동일한 WBS 번호를 브랜치·커밋·PR에 적습니다.

| 항목 | 형식 | 예시 |
| --- | --- | --- |
| 이슈 제목 | `[WBS번호] 작업명` | `[2.3.1] QR 검증 API 구현` |
| 브랜치 | `종류/WBS번호-작업명` | `feat/2.3.1-qr-validation` |
| 커밋 첫 줄 | `[머리말]_WBS번호/요약` | `[Add]_2.3.1/QrValidation` |
| PR 제목 | `[WBS번호] 작업명` | `[2.3.1] QR 검증 API 구현` |

브랜치 종류는 `feat`, `fix`, `infra`, `docs`, `test`, `refactor`, `chore`, `style`을 사용합니다. 커밋 머리말은 `[Add]`, `[Fix]`, `[Refactor]`, `[Docs]`를 사용합니다. 커밋 첫 줄 아래에 빈 줄을 두고 변경 내용을 적습니다.

기능 브랜치는 `develop`에서 만들고 작업 PR은 `develop`으로 보냅니다. `main` 반영은 `develop → main` PR로 진행합니다. 기본 브랜치인 `develop`으로 보내는 작업 PR에는 `Closes #12`를 사용합니다. `main` 반영 PR에서는 필요에 따라 `Refs #12`로 참조합니다. 여러 저장소에 걸친 이슈는 `Refs gonggongpublic/backend#12`처럼 저장소를 명시합니다.

API·이벤트·DB·배포 계약이 바뀌면 영향을 받는 담당자와 공유하고 관련 명세를 갱신합니다.
