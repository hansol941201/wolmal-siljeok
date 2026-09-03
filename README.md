# POUR 공사실적

브라우저에서 바로 여는 공개 주소입니다. 설치도 로그인도 필요 없습니다.

## https://hansol941201.github.io/wolmal-siljeok/

| 주소 | 무엇 |
|---|---|
| `/search/` | **공사실적 검색기** — 엑셀을 열어 공종·지역·연도·특허번호로 찾고 엑셀·CSV로 내보냅니다 |
| `/manage/` | **공사실적 관리** — K-APT 공고 등록 → 낙찰 전환 → 상세 관리 (예시 자료) |
| `/portfolio/POUR-portfolio-2024-2026.pdf` | **공사실적 자료** — 2024–2026 전국 1,171건, A4 37쪽 |

## 자료가 어디로 가는가

검색기에서 고른 엑셀은 **보는 사람의 컴퓨터 안에서만** 열립니다. 서버로
올라가지 않고, 이 저장소에도 담기지 않습니다. 관리 화면에서 입력한 내용도
그 브라우저에만 남고 다른 사람에게 전달되지 않습니다.

`/manage/` 에는 예시 자료 7건만 들어 있습니다. 실제 공사실적은 담겨 있지
않습니다.

## 고칠 때

`/search/` 와 `/manage/` 는 손으로 만든 파일이 아니라 원본 코드에서 만들어
낸 결과물입니다. **이 파일들을 직접 고치지 마세요.**

| 화면 | 원본 | 만드는 명령 |
|---|---|---|
| `/search/` | `hansol941201/pour-search` | `python3 build.py` (pour-html) |
| `/manage/` | `hansol941201/shin` 의 `pour-integration/` | `python3 pour-integration/scripts/build-preview.py` |

`main` 에 올리면 GitHub Actions 가 자동으로 다시 배포합니다.
