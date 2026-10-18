# VectraPath

> *Vector paths, engraved.*

**갈보(Galvo) 레이저 마킹을 위한 설계 · 데이터 · 내보내기 도구** (Windows)
Design · variable data · export tool for galvo laser marking.

로고 · 자동증가 시리얼 · 바코드를 올리고, N개로 배치하고, 마킹 순서를 정해서 —
**지금 쓰고 있는 마킹 SW(laserDESK · EZCAD · LightBurn · GRBL 등)에서 바로 여는 파일**로 내보냅니다.
레이저 장비 없이도 도면과 데이터를 끝까지 준비할 수 있습니다.

이 저장소는 **설치 파일 배포용**입니다(소스 코드는 포함하지 않습니다).

## 다운로드 · Download

👉 **[Releases](../../releases/latest)** 에서 최신 `VectraPath-x.y.z-setup.exe` 를 받으세요.

## 주요 기능 · Features

- 작도 · 편집: 선 · 사각형 · 원 · 타원 · 호 · 폴리라인 · 스플라인 · 텍스트, 스냅, 그룹, Undo/Redo
- 채움(해칭): Lines · ZigZag · CrossHatch · 테두리 오프셋 — 객체에 붙어 자동 재계산
- 바코드 10종: QR · DataMatrix · PDF417 · Aztec · Code128 · Code39 · EAN-13 · EAN-8 · UPC-A · ITF
- 가변 데이터: 시리얼 · 날짜 · CSV — 배열 사본마다 다음 값
- 배치: Array(N-up) · 정렬 · 분배 · 마킹 순서(최단 이동 · 행/열 · 지그재그)
- 가져오기 DXF · SVG / 내보내기 DXF · SVG · PLT · PDF · G-code
- (옵션) 카메라 · 비전: 웹캠 보정 · 화면 위 카메라 영상 · 기준 모양 찾기 → 정렬 내보내기 — 처음엔 꺼져 있음, `Settings › Use Vision (Camera)` 로 켜기
- 한국어 / English, 사용자 매뉴얼(PDF — Help › User Manual)

## 설치 · Install

- **요구 사항**: Windows 10/11 64비트, .NET Framework 4.8
- 설치 유형: 전체(비전 포함) / 기본(비전 제외). 기본 설치 위치는 이 사용자 폴더(관리자 권한 불필요) — 설치 시작 화면에서 "모든 사용자"로 바꿀 수 있습니다.
- **"Windows의 PC 보호" 경고**가 뜨면 아직 코드 서명 전이라서 그렇습니다 → **추가 정보 → 실행**.
- 받은 파일 확인: 각 릴리즈 노트의 **SHA256** 과 비교 (PowerShell `Get-FileHash 파일.exe`).

## 문의 · Feedback

버그 · 요청은 이 저장소의 **[Issues](../../issues)** 에 남겨 주세요.
오류가 났다면 설치 폴더의 `vectrapath.log`(기본 `%LocalAppData%\Programs\VectraPath`) 를 함께 첨부해 주시면 도움이 됩니다.

---
VectraPath 는 개인 프로젝트입니다(무료 공개 버전). 사용한 오픈소스 · 서드파티 고지는 설치 폴더의 `THIRD_PARTY_NOTICES.md` 를 참고하세요.
laserDESK · EZCAD · LightBurn 은 각 소유자의 상표입니다.
