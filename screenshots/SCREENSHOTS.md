# 홈페이지 스크린샷

`SiteScreenshotUITests`가 시뮬레이터(iPhone 17 Pro, iOS 26.5, 상태 바 9:41)에서 **언어 × 외관 4세트**를 자동으로 찍는다:
`ko-light/` `ko-dark/` `en-light/` `en-dark/` 아래 같은 이름의 PNG 23장(원본 1206×2622 → 절반 축소) + `thumbs/`(갤러리 정사각 212px).

## 갤러리 (git 기본 기능 — 순서는 `gen_site.py`의 `GALLERY`)

| 파일 | 화면 |
|---|---|
| `01-repo-list.png` | 저장소 목록 — 공개 리포 2개(gitignore, Starter-Kit-3D-Platformer, 얕은 클론) + nestling |
| `22-changes.png` | 변경 사항 탭 — 수정 1(docs/design.md) + 새 파일 1, 스테이지 전 |
| `03-changes-commit.png` | 커밋 시트 — 스테이지된 파일 + 메시지 |
| `04-history-graph.png` | 히스토리 그래프 — 머지 커밋, `v0.2.0` 태그 칩 |
| `21-commit-detail.png` | 커밋 상세 — 메시지·작성자·해시·바뀐 파일 |
| `05-diff-split.png` | 분할 diff (`src/player.gd`) |
| `07-branches.png` | 브랜치 시트 — 로컬·원격 브랜치 |
| `06-merge-editor.png` | 머지 에디터 — `feature/night-mode` 충돌 |
| `23-stash.png` | 변경 사항 보관(스태시) 시트 — 파일 체크리스트 |
| `02-files.png` | 파일 탭 (`src/`) |

## 강조 절

| 파일 | 화면 | 쓰이는 곳 |
|---|---|---|
| `02-files.png` + `10-files-app.png` | Roost 파일 탭의 `src/` ⇄ iOS 파일 앱에서 연 같은 `src/` (목록 보기 시도, 아무것도 고치기 전에 촬영) | "다른 앱과 함께 사용" |
| `11`~`20-viewer-*.png`, `08-viewers.png`, `09-viewers-fbx.png` | 코드·마크다운·Aseprite·이미지·FBX·오디오·Godot 씬·HTML·PDF·JSON·CSV·zip 뷰어 | "파일을 한 곳에서 편하게" 타일 12장(전체 비율) |

- 갤러리·타일은 페이지 언어 세트. 라이트/다크 토글은 `<html data-shots>`와 `localStorage("roost-shots")`로 세트 폴더만 바꾼다(`gen_site.py`의 `GALLERY_JS`).
- 다시 찍기: 전용 시뮬레이터에서 `ROOST_UITEST_SIM=<UDID> Scripts/run-uitests.sh SiteScreenshotUITests`(약 20분, 공개 리포 클론은 네트워크 필요)
  → `/tmp/roost-uitest/shots/site-<세트>-*.png` → 절반 축소·썸네일 생성해 위 폴더에. 파일 앱을 열고 나면 fileproviderd 복제본이
  남으므로 다음 실행 전에 기기를 지우거나(`simctl erase`) 새로 만든다.
- 샘플 리포 내용(커밋 메시지·README·주석)은 영어(`Scripts/make-sample-repo.py`, 2026-09-12).
- iPad 화면은 실기기에서만 — 필요하면 세트 폴더에 같은 이름으로 넣고 `gen_site.py`의 `GALLERY`에 항목을 더한다.
