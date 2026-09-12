# 홈페이지 스크린샷

`SiteScreenshotUITests`가 시뮬레이터(iPhone 17 Pro, iOS 26.5, 상태 바 9:41)에서 **언어 × 외관 4세트**를 자동으로 찍는다:
`ko-light/` `ko-dark/` `en-light/` `en-dark/` 아래 같은 이름의 PNG 7장(원본 1206×2622 → 절반 축소).

| 파일 | 화면 | 쓰이는 곳 |
|---|---|---|
| `01-repo-list.png` | 저장소 목록 — 공개 리포 2개(gitignore, Starter-Kit-3D-Platformer, 얕은 클론) + 즐겨찾기 nestling | 상단 스테이지(가운데), 갤러리 |
| `04-history-graph.png` | 히스토리 그래프 — 머지 커밋, `v0.2.0` 태그 칩 | 상단 스테이지(왼쪽), 갤러리 |
| `06-merge-editor.png` | 머지 에디터 — `feature/night-mode` 충돌, 앞뒤 맥락 | 상단 스테이지(오른쪽), 갤러리 |
| `05-diff-split.png` | 분할 diff (`src/player.gd`) | 갤러리 |
| `03-changes-commit.png` | 변경 사항 스테이지 + 커밋 시트 | 갤러리 |
| `02-files.png` | 파일 탭 (`assets/sprites`) | 갤러리 |
| `08-viewers.png` | Aseprite 뷰어 (타임라인 펼침) | 갤러리 |

- 상단 스테이지는 페이지 언어와 무관하게 **en 세트**, 갤러리는 페이지 언어 세트. 라이트/다크 토글은 `<html data-shots>`와 `localStorage("roost-shots")`로 세트 폴더만 바꾼다(`gen_site.py`의 `GALLERY_JS`).
- 다시 찍기: `Scripts/run-uitests.sh SiteScreenshotUITests`(약 10분, 공개 리포 클론은 네트워크 필요) → `/tmp/roost-uitest/shots/site-<세트>-*.png` → 절반 축소해 위 폴더에.
- 샘플 리포 내용(커밋 메시지·README·주석)은 영어(`Scripts/make-sample-repo.py`, 2026-09-12).
- 파일 앱(07)·iPad 화면은 실기기에서만 — 필요하면 세트 폴더에 같은 이름으로 넣고 `gen_site.py`의 `GALLERY`에 항목을 더한다.
