# SPINE X — Spine Graphic Study

전시용 인터랙티브 화면. 웹캠으로 손을 인식해 척추 수열(C · T · L · Ca)을 뽑고, 손동작으로 표본 형태를 변형한 뒤 도감에 등재한다.

## 실행
- `index.html` 과 `spinex_film.mp4` 를 같은 폴더에 두고 Chrome 으로 연다.
- 카메라 권한 허용 필요. MediaPipe 와 Pretendard 를 CDN 에서 불러오므로 인터넷 연결이 필요하다.
- 카메라가 없으면 키보드로 조작: `1` 생성 · `2–7` 모드 · `←→` 면 수 · `0` 대기. `D` 디버그 표시.

## 흐름
Show your open hand → Hold still → Make a fist (수열 확정) → 손동작으로 변형 → 손을 치우면 3초 후 End study → 등재

| 손동작 | 모드 |
|---|---|
| Fist | Base |
| Tilt palm | Mandala |
| Thumb + Index | Bleed |
| Thumb + Middle | Typographic |
| Thumb + Ring | Material |
| Thumb + Pinky | Inversion |

## 폰트
제목은 Eurostile Bold Extended(상용). 저장소에는 포함하지 않는다.
전시 PC 에 설치하거나 `fonts/EurostileBoldExtended.woff2` (또는 `.otf`) 로 넣어두면 적용된다. 없으면 Pretendard 로 대체.

## 영상
`spinex_film.mp4` 는 원본(116MB)을 1080p · H.264 로 재인코딩한 버전(약 14MB, 무음). 배경에 흐림 처리되어 깔린다.
